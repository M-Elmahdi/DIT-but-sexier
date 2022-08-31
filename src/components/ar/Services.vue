<template>
    <div class="container-xxl py-5" id="services">
      <div class="container">
        <div class="text-center mx-auto" style="max-width: 500px">
          <h1 class="display-6 mb-5 hacen-bold">
            {{ lang.services_title }}
          </h1>
        </div>
        <div class="row g-4 justify-content-center">
          <div class="col-lg-4 col-md-6 wow fadeInUp" data-wow-delay="0.1s">
            <div class="service-item rounded h-100 p-5">
              <div class="d-flex align-items-center ms-n5 mb-4">
                <div
                  class="service-icon flex-shrink-0 bg-primary rounded-end me-4"
                >
                  <img
                    class="img-fluid white-icon-svg"
                    src="@/assets/icons/parachute-box-solid.svg"
                    alt=""
                  />
                </div>
                <h4 class="mb-0 text-end hacen-regular">{{ lang.services_1_title }}</h4>
              </div>
              <p class="mb-4 fs-5 text-end">
                {{ lang.services_1_desc }}
              </p>
            </div>
          </div>
          <div class="col-lg-4 col-md-6 wow fadeInUp" data-wow-delay="0.3s">
            <div class="service-item rounded h-100 p-5">
              <div class="d-flex align-items-center ms-n5 mb-4">
                <div
                  class="service-icon flex-shrink-0 bg-primary rounded-end me-4"
                >
                  <img
                    class="img-fluid white-icon-svg"
                    src="@/assets/icons/server-solid.svg"
                    alt=""
                  />
                </div>
                <h4 class="mb-0 text-end hacen-regular">{{ lang.services_2_title }}</h4>
              </div>
              <p class="mb-4 fs-5 text-end">
                {{ lang.services_2_desc }}
              </p>
            </div>
          </div>
          <div class="col-lg-4 col-md-6 wow fadeInUp" data-wow-delay="0.5s">
            <div class="service-item rounded h-100 p-5">
              <div class="d-flex align-items-center ms-n5 mb-4">
                <div
                  class="service-icon flex-shrink-0 bg-primary rounded-end me-4"
                >
                  <img
                    class="img-fluid white-icon-svg"
                    src="@/assets/icons/chalkboard-teacher-solid.svg"
                    alt=""
                  />
                </div>
                <h4 class="mb-0 text-end hacen-regular">{{ lang.services_3_title }}</h4>
              </div>
              <p class="mb-4 fs-5 text-end">
                {{ lang.services_3_desc }}
              </p>
            </div>
          </div>
          <div class="col-lg-4 col-md-6 wow fadeInUp" data-wow-delay="0.1s">
            <div class="service-item rounded h-100 p-5">
              <div class="d-flex align-items-center ms-n5 mb-4">
                <div
                  class="service-icon flex-shrink-0 bg-primary rounded-end me-4"
                >
                  <img
                    class="img-fluid white-icon-svg"
                    src="@/assets/icons/sitemap-solid.svg"
                    alt=""
                  />
                </div>
                <h4 class="mb-0 text-end hacen-regular">{{ lang.services_4_title }}</h4>
              </div>
              <p class="mb-4 fs-5 text-end">
                {{ lang.services_4_desc }}
              </p>
            </div>
          </div>
          <div class="col-lg-4 col-md-6 wow fadeInUp" data-wow-delay="0.3s">
            <div class="service-item rounded h-100 p-5">
              <div class="d-flex align-items-center ms-n5 mb-4">
                <div
                  class="service-icon flex-shrink-0 bg-primary rounded-end me-4"
                >
                  <img
                    class="img-fluid white-icon-svg"
                    src="@/assets/icons/file-invoice-solid.svg"
                    alt=""
                  />
                </div>
                <h4 class="mb-0 text-end hacen-regular">{{ lang.services_5_title }}</h4>
              </div>
              <p class="mb-4 fs-5 text-end">
                {{ lang.services_5_desc }}
              </p>
            </div>
          </div>
          <div class="col-lg-4 col-md-6 wow fadeInUp" data-wow-delay="0.5s">
            <div class="service-item rounded h-100 p-5">
              <div class="d-flex align-items-center ms-n5 mb-4">
                <div
                  class="service-icon flex-shrink-0 bg-primary rounded-end me-4"
                >
                  <img
                    class="img-fluid white-icon-svg"
                    src="@/assets/icons/users-between-lines-solid.svg"
                    alt=""
                  />
                </div>
                <h4 class="mb-0 text-end hacen-regular">{{ lang.services_6_title }}</h4>
              </div>
              <p class="mb-4 fs-5 text-end">
                {{ lang.services_6_desc }}
              </p>
            </div>
          </div>
        </div>
      </div>
    </div>
</template>

<script>
export default {
    name: 'ArServices',
    props: {
      lang: Object,
    }
}
</script>
