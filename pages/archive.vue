<template>
  <div class="c-archive">
    <svg class="cursor" width="32" ref="cursor" height="32" viewBox="0 0 20 20">
      <circle class="cursor__inner" cx="10" cy="10" r="5" />
    </svg>
    <div class="c-archive__header">
      <nuxt-link to="/profile">
        <animated-link class="c-bezier">
          Profile
        </animated-link>
      </nuxt-link>
      <nuxt-link to="/">
        <animated-link class="c-bezier">
          Close
        </animated-link>
      </nuxt-link>
    </div>
    <LocomotiveScroll
      ref="scroller"
      class="horizontal"
      :getted-options="{
        direction: 'horizontal',
        smooth: true,
        getSpeed: true,
        lerp: 0.08
        // Other options
      }"
    >
      <div class="c-archive__main">
        <div>
          <div class="archive__intro">
            <p>
              This archive contains video clips, art and pictures related to
              Korty and her work, respective owners of each piece of work have
              been credited. Contact us for content removal
            </p>

            <button class="credits-link show-mobile" @click="openModal">
              <div class="c-inner">
                <animated-link class="c-bezier">
                  credits
                </animated-link>
              </div>
            </button>

            <h1>
              “I try not to do everything, but I make sure I try everything.”
            </h1>
            <nuxt-link to="/" class="home-link">
              <animated-link class="c-bezier">
                Go to Home
              </animated-link>
            </nuxt-link>

            <button class="credits-link show-desktop" @click="openModal">
              <div class="c-inner">
                <animated-link class="c-bezier">
                  credits
                </animated-link>
              </div>
            </button>
          </div>
          <div class="archive__images">
            <div class="c-image sm">
              <div
                data-scroll
                data-scroll-speed="-0.8"
                class="bg-image"
                style="background-image: url(https://res.cloudinary.com/dmwfd0zhh/image/upload/q_auto,f_auto/v1621637709/Korty/korty-archive-1_kjvsf4.jpg);"
              />
            </div>

            <div class="c-image xs">
              <div
                data-scroll
                data-scroll-speed="-0.8"
                class="bg-image"
                style="background-image: url(https://res.cloudinary.com/dmwfd0zhh/image/upload/q_auto,f_auto/v1621921598/Korty/Rectangle_25_wygie2.jpg);"
              />
            </div>

            <div class="c-image sm nobp">
              <div
                data-scroll
                data-scroll-speed="-0.8"
                class="bg-image"
                style="background-image: url(https://res.cloudinary.com/dmwfd0zhh/image/upload/q_auto,f_auto/v1621921685/Korty/Rectangle_34-1_firxdx.jpg);"
              />
            </div>

            <div class="c-image md nobp">
              <div
                data-scroll
                data-scroll-speed="-0.8"
                class="bg-image"
                style="background-image: url(https://res.cloudinary.com/dmwfd0zhh/image/upload/q_auto,f_auto/v1621921602/Korty/Rectangle_36_lj8azl.jpg);"
              />
            </div>

            <div class="c-image lg nobp">
              <div
                data-scroll
                data-scroll-speed="-0.8"
                class="bg-image"
                style="background-image: url(https://res.cloudinary.com/dmwfd0zhh/image/upload/q_auto,f_auto/v1621921624/Korty/Rectangle_37_er4jkv.jpg);"
              />
            </div>

            <div class="c-image md">
              <div
                data-scroll
                data-scroll-speed="-0.8"
                class="bg-image"
                style="background-image: url(https://res.cloudinary.com/dmwfd0zhh/image/upload/q_auto,f_auto/v1621921596/Korty/Rectangle_38_qtfbi4.jpg);"
              />
            </div>

            <div class="c-image xs">
              <div
                data-scroll
                data-scroll-speed="-0.8"
                class="bg-image"
                style="background-image: url(https://res.cloudinary.com/dmwfd0zhh/image/upload/q_auto,f_auto/v1621921620/Korty/Rectangle_39_bewtbe.jpg);"
              />
            </div>

            <div class="c-image sm">
              <div
                data-scroll
                data-scroll-speed="-0.8"
                class="bg-image"
                style="background-image: url(https://res.cloudinary.com/dmwfd0zhh/image/upload/q_auto,f_auto/v1621921686/Korty/Rectangle_40_ear7xg.jpg);"
              />
            </div>

            <div class="c-image sm">
              <div
                data-scroll
                data-scroll-speed="-0.8"
                class="bg-image"
                style="background-image: url(https://res.cloudinary.com/dmwfd0zhh/image/upload/q_auto,f_auto/v1621921677/Korty/Rectangle_42_md72qx.jpg);"
              />
            </div>

            <div class="c-image xs">
              <div
                data-scroll
                data-scroll-speed="-0.8"
                class="bg-image"
                style="background-image: url(https://res.cloudinary.com/dmwfd0zhh/image/upload/q_auto,f_auto/v1621921618/Korty/Rectangle_43_xhdyyi.jpg);"
              />
            </div>

            <div class="c-image xs">
              <div
                data-scroll
                data-scroll-speed="-0.8"
                class="bg-image"
                style="background-image: url(https://res.cloudinary.com/dmwfd0zhh/image/upload/q_auto,f_auto/v1621921643/Korty/Rectangle_44_crnxqk.jpg);"
              />
            </div>

            <div class="c-image md">
              <div
                data-scroll
                data-scroll-speed="-0.8"
                class="bg-image"
                style="background-image: url(https://res.cloudinary.com/dmwfd0zhh/image/upload/q_auto,f_auto/v1621921622/Korty/Rectangle_41_czd9h1.jpg);"
              />
            </div>

            <div class="c-image xs">
              <div
                data-scroll
                data-scroll-speed="-0.8"
                class="bg-image"
                style="background-image: url(https://res.cloudinary.com/dmwfd0zhh/image/upload/q_auto,f_auto/v1621921687/Korty/Rectangle_45_omfqqx.jpg);"
              />
            </div>

            <div class="c-image xs">
              <div
                data-scroll
                data-scroll-speed="-0.8"
                class="bg-image"
                style="background-image: url(https://res.cloudinary.com/dmwfd0zhh/image/upload/q_auto,f_auto/v1621921750/Korty/Rectangle_46_hwl8fv.jpg);"
              />
            </div>

            <div class="c-image sm">
              <div
                data-scroll
                data-scroll-speed="-0.8"
                class="bg-image"
                style="background-image: url(https://res.cloudinary.com/dmwfd0zhh/image/upload/q_auto,f_auto/v1621921644/Korty/Rectangle_47_nesabh.jpg);"
              />
            </div>

            <div class="c-image xs">
              <div
                data-scroll
                data-scroll-speed="-0.8"
                class="bg-image"
                style="background-image: url(https://res.cloudinary.com/dmwfd0zhh/image/upload/q_auto,f_auto/v1621921680/Korty/Rectangle_48_ybbj09.jpg);"
              />
            </div>

            <div class="c-image xs">
              <div
                data-scroll
                data-scroll-speed="-0.8"
                class="bg-image"
                style="background-image: url(https://res.cloudinary.com/dmwfd0zhh/image/upload/q_auto,f_auto/v1621921727/Korty/Rectangle_56_k6qgpk.jpg);"
              />
            </div>

            <div class="c-image lg">
              <div
                data-scroll
                data-scroll-speed="-0.8"
                class="bg-image"
                style="background-image: url(https://res.cloudinary.com/dmwfd0zhh/image/upload/q_auto,f_auto/v1621921640/Korty/Rectangle_49_taxh6a.jpg);"
              />
            </div>

            <div class="c-image sm nobp">
              <div
                data-scroll
                data-scroll-speed="-0.8"
                class="bg-image"
                style="background-image: url(https://res.cloudinary.com/dmwfd0zhh/image/upload/q_auto,f_auto/v1621921695/Korty/Rectangle_50_m3cic3.jpg);"
              />
            </div>

            <div class="c-image xs nobp">
              <div
                data-scroll
                data-scroll-speed="-0.8"
                class="bg-image"
                style="background-image: url(https://res.cloudinary.com/dmwfd0zhh/image/upload/q_auto,f_auto/v1621921794/Korty/Rectangle_51_mj4vqi.jpg);"
              />
            </div>

            <div class="c-image xs">
              <div
                data-scroll
                data-scroll-speed="-0.8"
                class="bg-image"
                style="background-image: url(https://res.cloudinary.com/dmwfd0zhh/image/upload/q_auto,f_auto/v1621921702/Korty/Rectangle_52_r0cnkm.jpg);"
              />
            </div>

            <div class="c-image md">
              <div
                data-scroll
                data-scroll-speed="-0.8"
                class="bg-image"
                style="background-image: url(https://res.cloudinary.com/dmwfd0zhh/image/upload/q_auto,f_auto/v1621921704/Korty/Rectangle_53_k2chip.jpg);"
              />
            </div>

            <div class="c-image xs">
              <div
                data-scroll
                data-scroll-speed="-0.8"
                class="bg-image"
                style="background-image: url(https://res.cloudinary.com/dmwfd0zhh/image/upload/q_auto,f_auto/v1621921770/Korty/Rectangle_54_r0rsvh.jpg);"
              />
            </div>

            <!-- Copy Image -->

            <div class="c-image md">
              <div
                data-scroll
                data-scroll-speed="-0.8"
                class="bg-image"
                style="background-image: url(https://res.cloudinary.com/dmwfd0zhh/image/upload/q_auto,f_auto/v1621921773/Korty/Rectangle_57_twgrjb.jpg);"
              />
            </div>

            <div class="c-image xs">
              <div
                data-scroll
                data-scroll-speed="-0.8"
                class="bg-image"
                style="background-image: url(https://res.cloudinary.com/dmwfd0zhh/image/upload/q_auto,f_auto/v1621921708/Korty/Rectangle_55_eequ72.jpg);"
              />
            </div>

            <div class="c-image xs">
              <div
                data-scroll
                data-scroll-speed="-0.8"
                class="bg-image"
                style="background-image: url(https://res.cloudinary.com/dmwfd0zhh/image/upload/q_auto,f_auto/v1621921722/Korty/Rectangle_58_kiisqn.jpg);"
              />
            </div>

            <div class="c-image xs">
              <div
                data-scroll
                data-scroll-speed="-0.8"
                class="bg-image"
                style="background-image: url(https://res.cloudinary.com/dmwfd0zhh/image/upload/q_auto,f_auto/v1621921759/Korty/Rectangle_59_tjr5nx.jpg);"
              />
            </div>

            <div class="c-image sm">
              <div
                data-scroll
                data-scroll-speed="-0.8"
                class="bg-image"
                style="background-image: url(https://res.cloudinary.com/dmwfd0zhh/image/upload/q_auto,f_auto/v1621921782/Korty/Rectangle_60_bwxjnj.jpg);"
              />
            </div>

            <div class="c-image lg">
              <div
                data-scroll
                data-scroll-speed="-0.8"
                class="bg-image"
                style="background-image: url(https://res.cloudinary.com/dmwfd0zhh/image/upload/q_auto,f_auto/v1621921812/Korty/Rectangle_61_hgeq0v.jpg);"
              />
            </div>

            <div class="c-image lg">
              <div
                data-scroll
                data-scroll-speed="-0.8"
                class="bg-image"
                style="background-image: url(https://res.cloudinary.com/dmwfd0zhh/image/upload/q_auto,f_auto/v1621921816/Korty/Rectangle_62_zkkzof.jpg);"
              />
            </div>

            <div class="c-circle">
              <div class="c-circle__inner">
                <div class="heading">
                  <h3>
                    the <br />
                    End
                  </h3>
                </div>

                <nuxt-link to="/" class="home-link">
                  <animated-link class="c-bezier">
                    Go to Home
                  </animated-link>
                </nuxt-link>
              </div>
            </div>

            <div class="c-image xs">
              <div
                data-scroll
                data-scroll-speed="-0.8"
                class="bg-image"
                style="background-image: url(https://res.cloudinary.com/dmwfd0zhh/image/upload/q_auto,f_auto/v1621921814/Korty/Rectangle_64_v1mfrj.jpg);"
              />
            </div>
          </div>
        </div>
      </div>
    </LocomotiveScroll>
  </div>
</template>

<script>
import AnimatedArrow from "@/components/AnimatedArrow.vue";
import AnimatedLink from "@/components/AnimatedLink/AnimatedLink.vue";
import { map, clamp } from "@/utils/index";
import gsap from "gsap/all";
import { Cursor } from "~/animations/cursor";

export default {
  components: { AnimatedArrow, AnimatedLink },

  /**
   * TODO: outsource the exit animations into one and reuse
   */
  transition: {
    name: "profile",
    mode: "out-in",
    css: false,
    appear: true,
    beforeEnter(el) {
      gsap.set(el, {
        opacity: 0
      });
    },
    enter(el, done) {
      const tl = gsap.timeline({
        onComplete: done
      });
      tl.to(el, {
        opacity: 1,
        duration: 1.5
      })
        .set(".archive__images .c-image", { autoAlpha: 1 }, "-=1.5")
        .from(
          ".archive__images .c-image",
          {
            duration: 1.5,
            yPercent: 100,
            ease: "Expo.easeInOut"
          },
          "-=1.5"
        )
        .from(".archive__images .bg-image", {
          duration: 1.5,
          yPercent: -100,
          delay: -1.5,
          ease: "Expo.easeInOut"
        })
        .from(".archive__images .bg-image", {
          duration: 1.5,
          scale: 1.2,
          delay: -1.4,
          ease: "Expo.easeInOut"
        });
    },
    beforeLeave(el) {
      gsap.set(".c-exit", {
        zIndex: 30,
        top: "unset",
        bottom: 0
      });
      gsap.set(".exit-span", {
        opacity: 1
      });
    },
    leave(el, done) {
      const tl = gsap.timeline({
        onComplete: done
      });

      tl.to(".c-exit", {
        height: window.innerHeight,
        duration: 1.5,
        ease: "Expo.easeInOut"
      })
        .set(".c-exit", {
          top: 0,
          bottom: "unset"
        })
        .from(
          ".exit-span",
          {
            yPercent: 100,
            duration: 1,
            skewY: 5,
            stagger: {
              amount: 0.1
            },
            ease: "power2.out"
          },
          "-=.5"
        )
        .set(el, {
          opacity: 0
        })
        .to(".exit-span", {
          opacity: 0,
          duration: 1,
          ease: "power2.out"
        })
        .to(
          ".c-exit",
          {
            height: 0,
            duration: 1.5,
            ease: "Expo.easeInOut"
          },
          "-=1"
        );
    }
  },
  mounted() {
    const locomotive = this.$refs.scroller.locomotive;
    this.$nuxt.$emit("update-locomotive");
    this.beginCursor();

    let direction = "horizontal";
    window.addEventListener("resize", () => {
      const width = window.innerWidth;

      if (width <= 768 && direction !== "vertical") {
        locomotive.destroy();
        locomotive.init();
        direction = "vertical";
      }

      if (width > 768 && direction === "vertical") {
        locomotive.destroy();
        locomotive.init();
        direction = "horizontal";
      }
    });

    let scroll = { cache: 0, current: 0 };
    const allImgs = [...document.querySelectorAll(".archive__images .c-image")];
    locomotive.on("scroll", obj => {
      scroll.current = obj.scroll.x;
      const distance = scroll.current - scroll.cache;
      scroll.cache = scroll.current;
      const skewVal = map(distance, -50, 50, -15, 15);
      allImgs.forEach(
        el => (el.style.transform = `skewX(${clamp(skewVal, -1, 1)}deg)`)
      );
    });
    locomotive.update();
  },
  methods: {
    openModal() {
      this.$store.commit("updateModal", true);
    },
    beginCursor() {
      const cursorRef = this.$refs.cursor;
      const cursor = new Cursor(cursorRef);
      [...document.querySelectorAll("a")].forEach(link => {
        link.addEventListener("mouseenter", () => cursor.enter());
        link.addEventListener("mouseleave", () => cursor.leave());
      });
      [...document.querySelectorAll("button")].forEach(link => {
        link.addEventListener("mouseenter", () => cursor.enter());
        link.addEventListener("mouseleave", () => cursor.leave());
      });
    }
  }
};
</script>

<style lang="scss" scoped></style>
