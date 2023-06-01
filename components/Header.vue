<template>
    <div class="w-full">
        <nav class="fixed flex flex-row items-center justify-between px-10 w-full  bg-black bg-opacity-10 z-10 drop-shadow-lg py-5">
            <div class="flex flex-row">
                <img src="/Vector.png" class="w-8 mx-6 hover:bg-[#F79327] cursor-pointer" >
                <span class="text-white px-2 text-[25px] font-arial cursor-pointer hover:text-[#F79327]" to="/" >Airbnb</span>
            </div>
            <div class="flex items-center text-white px-5 space-x-5 drop-shadow-2xl">
                <NuxtLink to="/" class="hover:text-[#F79327]">Français (FR)</NuxtLink>
                <NuxtLink to="/" class="hover:text-[#F79327]">EUR €</NuxtLink>
                <NuxtLink to="/" class="hover:text-[#F79327]">Devenir hôte</NuxtLink>
                <NuxtLink to="/" class="hover:text-[#F79327]">Créer son expérience</NuxtLink>
                <NuxtLink to="/" class="hover:text-[#F79327]">Aide</NuxtLink>
                <NuxtLink to="/" class="hover:text-[#F79327]">Inscription</NuxtLink>
                <NuxtLink to="/" class="hover:text-[#F79327]">Connexion</NuxtLink>
            </div>
        </nav>

        <div class="w-full">
            <img src="/Hero.png" class="md:mx-auto w-full">
            <div class="md:absolute bg-white rounded-lg left-72 top-24 py-10 px-6 w-[500px]">
                <h1 class="text-black font-semibold text-[30px] w-80">Réservez des hébergements et des activités uniques.</h1>
                <div class="w-96 mt-10 uppercase text-md ">
                    <span>Où</span>
                    <input type="text" class="border p-2 mt-1 border-red-200 block bg-white rounded-md  w-[435px] shadow-lg placeholder:text-slate-400"  placeholder="Partout">
                </div>

                <div class="w-96 mt-10 uppercase text-md flex flex-col">
                    <div class="justify-between space-x-[180px]">
                        <span>Arrivée</span>
                        <span>Départ</span>
                    </div>
                    <div class="justify-between mt-1 space-x-1 w-[500px]">
                        <input class="border border-red-200 shadow-lg p-2 w-60 pl-4 pb-3 rounded-md" type="date">
                        <input class="border border-red-200 shadow-lg p-2 w-[190px] pl-10 pb-3 rounded-md" type="time">
                    </div>
                </div>

                
                <div class="w-96 mt-8 uppercase text-md ">
                    <span>Voyageurs</span>
                    <input type="text" class="border p-2 mt-1 border-red-200 block bg-white rounded-md  w-[435px] shadow-lg placeholder:text-slate-400"  placeholder="Voyageurs">
                </div>

                <button class=" float-right mr-4 rounded-md mt-8 p-4 pl-12 pr-12 bg-red-500 text-white items-center hover:scale-110">
                    Rechercher
                </button>
            </div>

         </div>
    </div>
</template>

<script setup>

</script>
