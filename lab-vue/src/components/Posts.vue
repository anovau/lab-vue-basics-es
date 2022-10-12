<template>
    <div v-for="content in dataArray" class="container content-div">
        <div class="card mt-3">
            <div class="card-content">
                <div class="media">
                    <div class="media-content">
                        <p class="title is-4">{{content.title}}</p>
                        <p class="subtitle is-6">{{content.description}}</p>
                    </div>
                </div>

                <div class="content">
                    {{content.content}}
                </div>
            </div>
        </div>
    </div>
</template>
<script setup>

const dataArray = [
    {
        title: "Titulo uno",
        decription: "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ut efficitur.",
        content: "Ut vel urna in eros molestie fermentum sed sed felis. Fusce turpis purus, vehicula vel condimentum at, pulvinar ut urna. Nullam quis dolor vel risus ornare hendrerit. Etiam sed condimentum justo. Sed semper mauris vitae tincidunt convallis. Suspendisse feugiat nisl in augue commodo iaculis. Proin ultricies mauris quis lacus elementum suscipit."
    },
    {
        title: "Titulo dos",
        decription: "Aliquam erat volutpat. In nulla mauris, consectetur eu nibh sed, placerat congue turpis.",
        content: "Pellentesque non feugiat ex. Phasellus suscipit lorem sapien, ac imperdiet nulla bibendum in. Sed congue lorem sit amet urna vulputate ultricies. Aliquam dictum, dolor non convallis placerat, turpis magna euismod urna, sed euismod leo augue in mauris."
    },
    {
        title: "Titulo tres",
        decription: "Sed quis lectus vel arcu sodales fringilla.",
        content: "Praesent egestas felis vel elit ullamcorper hendrerit. Donec ornare ante quis eros auctor, id tempus mauris volutpat. Mauris commodo magna at mi fermentum, et eleifend felis auctor. Donec volutpat elementum dignissim. "
    }
]


</script>
<style scoped>
.content-div {
    display: flex;
    justify-content: center;
    align-items: center;
}

</style>