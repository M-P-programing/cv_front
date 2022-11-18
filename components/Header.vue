<template>
  <div>
    <header class="w-100 bg-secondary">
      <nav class="">
        <div class="uppercase">
          <ul class="font-bold text-sm h-20 grid grid-cols-5 text-white">
            <li class="text-center border-r border-black pt-7 hover:bg-primary duration-500 cursor-pointer">
              <a href="#about" class="">{{ $t("header.about") }}</a>
            </li>
            <li class="text-center border-r border-black pt-7 hover:bg-primary duration-500 cursor-pointer">
              <a href="#" class="">{{ $t("header.resume") }}</a>
            </li>
            <li class="text-center border-r border-black pt-7 hover:bg-primary duration-500 cursor-pointer">
              <a href="#" class="">{{ $t("header.download_my_cv") }}</a>
            </li>
            <li class="text-center border-r border-black pt-7 hover:bg-primary duration-500 cursor-pointer">
              <a href="#" class="">{{ $t("header.my_skills") }}</a>
            </li>
            <li class="text-center border-r border-black pt-7 hover:bg-primary duration-500 cursor-pointer">
              <a href="#" class="">{{ $t("header.contact_me") }}</a>
            </li>
          </ul>
        </div>
      
      </nav>
    </header>
  </div>
</template>

<script>
export default {
  computed: {
    availableLocales() {
      return this.$i18n.locales.filter((i) => i.code !== this.$i18n.locale);
    },
  },
};
</script>