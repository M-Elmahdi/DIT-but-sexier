<template>
    <div class="container-fluid overflow-hidden my-5 px-lg-0" id="vision">
      <div class="container facts px-lg-0">
        <div class="row g-0 mx-lg-0 text-end">
          <div class="col-lg-6 facts-text wow fadeIn pe-5" data-wow-delay="0.1s">
            <div class="h-100 px-4 ps-lg-0">
              <h1 class="text-white mb-4 hacen-regular">{{ lang.vision_title }}</h1>
              <p class="text-light hacen-regular h5 mb-5">
                {{ lang.vision_desc }}
              </p>
            </div>
          </div>
          <div class="col-lg-6 wow fadeIn" data-wow-delay="0.5s">
            <div class="h-100 px-4 pe-lg-0">
              <div class="row g-5">
                  <div class="text-light hacen-bold text-center text-dark fs-2 mb-1">
                    شركائنا
                  </div>
                  <img src="@/assets/img/partners_section.png" class="mt-0" />
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
</template>

<script>
export default {
    name: 'ArVision',
    props: {
      lang: Object,
    }
}
</script>

<style>

</style>
