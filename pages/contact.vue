<template>
  <div>
    <section class="py-10">
      <div class="container m-auto grid lg:grid-cols-2 gap-5 items-center">
        <div>
          <h1 class="text-3xl font-bold">{{ companyStore.company.name }}</h1>
          <address>
            {{ companyStore.company.address }} <br />
            {{ companyStore.company.contact }} <br />
            {{ companyStore.company.email }} <br />
          </address>
        </div>
        <div>
          <iframe
            src="https://www.google.com/maps/embed?pb=!1m14!1m8!1m3!1d14242.648482944307!2d87.2862987!3d26.8188851!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x39ef4175e4f26a95%3A0x9b8526c7c4c7bc1c!2sCode%20IT!5e0!3m2!1sen!2snp!4v1689836218813!5m2!1sen!2snp"
            width="600"
            height="450"
            style="border: 0"
            allowfullscreen=""
            loading="lazy"
            referrerpolicy="no-referrer-when-downgrade"
          ></iframe>
        </div>
      </div>
    </section>
  </div>
</template>

<script setup>
import { useCompanyStore } from "~/store/company";
const companyStore = useCompanyStore();
</script>

<style lang="scss" scoped>
</style>