<script setup>
import AppHeader from "../components/AppHeader.vue";
import AppSectionTitle from "../components/AppSectionTitle.vue";
import profileCard from "../components/sp-aice/profileCard.vue";
import { RouterLink } from "vue-router";
import ProjectCards from "../components/sp-aice/ProjectCards.vue";
import SpaiceIcon from "../components/icons/SpaiceIcon.vue";
</script>

<template>
  <AppHeader class="flex-grow-0 flex-shrink-0"
    ><div
      class="p-2 bg-neutral-900 bg-opacity-75 rounded-lg shadow whitespace-nowrap flex gap-2"
    >
      <SpaiceIcon /> SP-AICE
    </div></AppHeader
  >
  <main class="flex-grow">
    <AppSectionTitle name="Team" />
    <div
      class="grid grid-flow-row md:grid-cols-2 2xl:grid-cols-4 mx-auto gap-12"
    >
      <profileCard
        memberName="Axel"
        description="Musik är något Axel tycker förgyller livet. Dela gärna med dig vilken musik du gillar och om du själv spelar något instrument."
        imageName="members/Axel2.jpg"
        imageAlt="Picture of member Axel"
        githubLink="https://github.com/axelhagerback"
      />
      <profileCard
        memberName="Isac"
        description="Om du börjar prata  träning med Isac kommer du inte bli av med honom på ett tag"
        imageName="members/Isac1.jpg"
        imageAlt="Picture of member Isac"
        summary="Hej hej jag heter Isac"
        githubLink="https://github.com/isacchr"
      />
      <profileCard
        memberName="Casper"
        description="Casper är norsk, han är dansk, han är lite allt möjligt. Precis som hans intressen och ämnen att diskutera."
        imageName="members/Casper2.jpg"
        imageAlt="Picture of member Casper"
        githubLink="https://github.com/CasperHogstrom"
      />
      <profileCard
        memberName="Elliot"
        description="En bra arbetsplats kan variera för Elliot, antingen kontor eller vid hans hund Milo."
        imageName="members/Elliot2.jpg"
        imageAlt="Picture of member Elliot"
        githubLink="https://github.com/elliotabrahamsson"
      />
    </div>
    <section
      class="space-y-4 mx-auto w-[380px] md:w-[768px] xl:w-[1156px] 2xl:w-[1544px] max-w-full"
    >
      <h1 class="text-center font-bold text-4xl">Projekt</h1>
      <div>
        <ProjectCards
          name="Mind Dump"
          description="Mind Dump är en webbapplikation
    som man kan skapa anteckningar för sina behov. Den erbjuder funktioner som att
    ta bort och redigera nuvarande anteckningar."
          :images="[
            'mind_dump/Screenshot_6.png',
            'mind_dump/Screenshot_2.png',
            'mind_dump/Screenshot_3.png',
            'mind_dump/Screenshot_4.png',
            'mind_dump/Screenshot_5.png',
          ]"
        />
      </div>
    </section>
  </main>
</template>
