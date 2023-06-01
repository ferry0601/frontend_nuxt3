<template>
  <div>
    <Header />
    <div class="flex flex-col pb-6 mt-10">
      <span class="text-[30px] font-bold mx-32 p-5">Explorer Airbnb</span>
      <div class="w-full flex flex-row justify-center space-x-32">
                <div v-for="card in cardbox" :key="card">
                  <Explorer :card = "card"/>
                </div>
      </div>
    </div>

    <div class="flex flex-col w-full">
    <div class="mt-32 mx-40">
          <span class="text-[30px] font-extrabold">Hébergements Airbnb Plus</span>
          <p class="font-light w-[550px]">Une sélection de logements vérifiés selon des critères de qualité et de design</p>
      </div>
      <div class=" mt-4 mx-40 mb-60">
        <img src="/Rectangle5.png" class=" w-[1380px] sm:absolute">
        <img src="/big-logo.png" class="w-32 mx-[600px] my-[1450px] sm:absolute justify-center object-cover leading-6 top-0">
        <button type="submit" class="mx-[550px] my-[220px] sm:absolute bg-white text-black rounded-md drop-shadow-xl border p-5 cursor-pointer hover:scale-110">
          <span>Découvrir des logements </span>
          <Icon name="material-symbols:arrow-right-alt" size="20" />

        </button>
      </div>
      
    </div>

    <div class="w-full flex flex-col mt-32">
      <div class="mt-6 mx-40">
          <span class="text-[30px] font-extrabold">Découvrez les aventures Airbnb</span>
          <p class="font-light w-[550px]">Voyages de plusieurs jours organisés par des experts locaux avec activités, repas et logements compris</p>
      </div>

      <div class="grid grid-cols-6 mt-6 w-[1400px] items-center mx-40 drop-shadow-lg pb-2">
        <div v-for="itemb in itembox" :key="itemb">
          <Aventure :itemb = "itemb" />
        </div>
      </div>
    </div>
  </div>
  <Footer/>
</template>

<script setup>
  const cardbox = [
        { id: 1, name: 'Logements', img : '/img24.png' },
        { id: 2, name: 'Expériences', img: '/img25.png' },
        { id: 3, name: 'Aventures', img: '/img26.png' }
    ]

  const itembox = [
        {
          id: 1, location: 'Cayman Islands', name: '2 Nights PACKAGE All Inclusive', 
          desc: 'À partir de 577€/personne - 3 jours', rate: '5.0', img: '/img1.png'
        },
        {
          id: 2, location: 'Uruguay', name: '2 Nights PACKAGE All Inclusive',
          desc: 'À partir de 577€/personne - 3 jours', rate: '5.0', img: '/img2.png'
        },
        {
          id: 3, location: 'Iceland', name: '2 Nights PACKAGE All Inclusive',
          desc: 'À partir de 577€/personne - 3 jours', rate: '5.0', img: '/img3.png'
        },
        {
          id: 4, location: 'Mongolia', name: '2 Nights PACKAGE All Inclusive',
          desc: 'À partir de 577€/personne - 3 jours', rate: '5.0', img: '/img4.png'
        },
        {
          id: 5, location: 'Bahrain', name: '2 Nights PACKAGE All Inclusive',
          desc: 'À partir de 577€/personne - 3 jours', rate: '5.0', img: '/img5.png'
        },
        {
          id: 6, location: 'Bosnia and Herzegovina', name: '2 Nights PACKAGE All Inclusive',
          desc: 'À partir de 577€/personne - 3 jours', rate: '5.0', img: '/img6.png'
        },
  ]
</script>
