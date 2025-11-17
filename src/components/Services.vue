<template>
  <section class="text-white mt-20" id="services">
    <div class="px-4 xl:pl-16">
      <h2 class="text-4xl font-bold text-white mb-4">My Services</h2>
    </div>
    <div
      class="py-8 xl:px-16 px-4 sm:py-16 grid grid-cols-1 gap-6 pt-10 sm:grid-cols-2 md:gap-10 md:pt-12 lg:grid-cols-3"
    >
      <div
        v-for="service in services"
        :key="service.id"
        data-aos="fade-up"
        class="px-8 py-12 rounded-xl bg-[#111a3e] shadow-lg border border-[#1f1641]"
      >
        <div class="mx-auto h-24 text-center xl;h-28 xl:w-28">
          <div>
            <img :src="service.icon" alt="icon service" />
          </div>
          <div class="text-center">
            <h3
              class="pt-8 text-lg font-semibold uppercase text-transparent bg-clip-text bg-gradient-to-r from-primary to-secondary lg:text-xl"
            >
              {{ service.name }}
            </h3>
            <p
              class="text-grey pt-4 text-sm group-hover:text-white md:text-base"
            >
              {{ service.description }}
            </p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
<script setup>
import { ref } from "vue";

const services = ref([
  {
    id: 1,
    icon: "google-code.png",
    name: "Web Development",
    description:
      "Lorem ipsum dolor, sit amet consectetur adipisicing elit. Temporibus dicta vero alias quis consectetur exercitationem!",
  },
  {
    id: 2,
    icon: "external-technical-writing-mobile-app-development-glyph-vectorslap.png",
    name: "Technical Writing",
    description: "Lorem ipsum dolor, sit amet consect",
  },
  {
    id: 3,
    icon: "external-mobile-development-digital-marketing-solid-design-circle.png",
    name: "Mobile Development",
    description: "Lorem ipsum dolor, sit amet consect",
  },
  {
    id: 4,
    icon: "email-open.png",
    name: "Web Design",
    description:
      "Lorem ipsum dolor, sit amet consect, ipsum dolor, sit amet consect",
  },
  {
    id: 5,
    icon: "windows10-personalization.png",
    name: "Graphic Design",
    description:
      "Lorem ipsum dolor, sit amet consect, ipsum dolor, sit amet consect",
  },
  {
    id: 6,
    icon: "web-design.png",
    name: "Web Designing",
    description:
      "Lorem ipsum dolor, sit amet consect, ipsum dolor, sit amet consect",
  },
]);
</script>
