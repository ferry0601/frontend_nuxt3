<template>
    <div class="w-full">
        
        <div class="p-5 md:flex pl-0 pt-0 pb-0 pr-40 drop-shadow-xl flex-row bg-white border rounded-xl cursor-pointer hover:scale-110">
            <img class="md:rounded w-24 h-24" :src="card.img" >

            <div class="w-full items-center pl-10 mt-10">
                <span class="text-black">{{ card.name }}</span>
            </div>
        </div>
    </div>
</template>

<script setup>
    const props = defineProps(['card'])
    const {card} = toRefs(props)
</script>
