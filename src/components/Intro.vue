<template>
  <div
    class="flex h-screen-80 max-w-7xl m-center mt-24 md:flex-col lg:flex-row md:pt-10"
  >
    <div class="info flex flex-col items-start lg:w-3/6 m-auto">
      <h2
        data-aos="fade-right"
        data-aos-delay="500"
        data-aos-duration="500"
        class="text-5xl pb-3 font-extrabold f-black name dark:text-white duration-1000"
      >
        John Ryan Inoc
      </h2>
      <h4
        class="text-lg pb-2 f-gray dark:text-white duration-1000"
        data-aos="fade-right"
        data-aos-delay="700"
        data-aos-duration="500"
      >
        BSIT 3rd Year Student
      </h4>
      <h5
        class="text-sm pb-12 f-gray dark:text-white duration-1000"
        data-aos="fade-right"
        data-aos-delay="800"
        data-aos-duration="500"
      >
        You know, I'm all about that education and never-ending learning
        journey. Whenever there's a challenge in my academic path, you can bet
        I'm diving right in. But it's not just about tackling what's in front of
        me; I'm all about hunting down chances to beef up my skill set too.
      </h5>
      <div
        data-aos="fade-right"
        data-aos-delay="800"
        data-aos-duration="700"
      ></div>
    </div>
    <img
      data-aos="zoom-in-right"
      data-aos-delay="800"
      data-aos-duration="800"
      class="m-auto clipped light imedium img-center md:w-auto"
      src="../assets/img/self/self.jpg"
      alt=""
      width="400"
    />
  </div>
</template>

<style lang="scss" scoped>
.clipped {
  clip-path: polygon(
    30% 0%,
    70% 0%,
    100% 30%,
    100% 70%,
    70% 100%,
    30% 100%,
    0% 70%,
    0% 30%
  );
}

.imedium {
  height: 25rem;
}

.light {
  filter: grayscale(40%);
  transition: 0.2s ease-out 10ms;
  cursor: pointer;

  &:hover {
    filter: grayscale(0);
    transform: scale(1.03);
    z-index: 999;
  }

  &.colored {
    filter: grayscale(0) !important;
  }
}

.profile-image {
  &::after {
    content: "";
    position: absolute;
    bottom: 120px;
    background: rgba(80, 80, 80, 0.503);
    width: 25rem;
    height: 50px;
    border-radius: 50%;
    filter: blur(20px);
    margin-left: 6rem;
  }
}

@media (max-width: 768px) {
  .imedium {
    display: none;
  }
}
</style>
