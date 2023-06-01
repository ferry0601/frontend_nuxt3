<template>
    <div class="items-center justify-center mb-10">
        <div class="flex flex-col bg-white drop-shadow-lg w-[188px] pb-4 cursor-pointer hover:scale-110">
            <img :src="itemb.img" class=" md:rounded h-[240px] w-[188px] drop-shadow-xl justify-center items-center">
            <span class="text-xs font-light text-gray-900 pl-2 mt-2">
                {{ itemb.location }}
            </span>

            <span class="items-center text-md font-bold pl-2">
                {{ itemb.name }}
            </span>

            <span class="items-center text-sm font-light pl-2">
                {{ itemb.desc }}
            </span>

            <span class="items-center text-sm font-light flex flex-row pl-2">
                {{ itemb.rate }}
                <img src="/star.png" class="justify-end ml-1" >
            </span>


        </div>
    </div>
</template>

<script setup>
    const props = defineProps(['itemb'])
    const {itemb} = toRefs(props)
</script>
