<template>
  <section class="testimonials">
    <div class="testimonials-image">
      <img src="../assets/images/illustration-stay-productive.png" />
    </div>
    <div class="testimonials-content">
      <h1>Stay productive, wherever you are</h1>
      <p class="text-1">
        Never let location be an issue when accessing your files, Fylo has you
        covered for all of your life storage needs
      </p>
      <p class="text-2">
        Securely share files and folders with friends, family and colleagues for
        live collaboration. No email attachments required.
      </p>
      <div class="testimonials-link">
        <a>See how Fylo works</a>
        <svg
          width="16"
          height="16"
          xmlns="http://www.w3.org/2000/svg"
          xmlns:xlink="http://www.w3.org/1999/xlink"
        >
          <defs>
            <circle id="b" cx="6" cy="6" r="6" />
            <filter
              x="-25%"
              y="-25%"
              width="150%"
              height="150%"
              filterUnits="objectBoundingBox"
              id="a"
            >
              <feOffset in="SourceAlpha" result="shadowOffsetOuter1" />
              <feGaussianBlur
                stdDeviation="1"
                in="shadowOffsetOuter1"
                result="shadowBlurOuter1"
              />
              <feColorMatrix
                values="0 0 0 0 0.384313725 0 0 0 0 0.878431373 0 0 0 0 0.850980392 0 0 0 0.811141304 0"
                in="shadowBlurOuter1"
              />
            </filter>
          </defs>
          <g fill="hsl(0, 0%, 100%)" fill-rule="evenodd">
            <g transform="translate(2 2)">
              <use fill="#000" filter="url(#a)" xlink:href="#b" />
              <use fill="" xlink:href="#b" />
            </g>
            <path
              d="M8.582 6l-.363.35 1.452 1.4H5.333v.5h4.338L8.22 9.65l.363.35 2.074-2z"
              fill="#1B2330"
            />
          </g>
        </svg>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "Testimonials",
};
</script>

<style>
.testimonials {
  display: flex;
  justify-content: center;
  gap: 5rem;
  font-family: "Raleway", sans-serif;
}

.testimonials-content {
  color: hsl(0, 0%, 100%);
  margin-top: 8rem;
}

.testimonials-content h1 {
  font-weight: 700;
  font-size: 2.7rem;
  width: 30rem;
}

.testimonials-content p {
  font-weight: 400;
  font-size: 0.9rem;
  width: 32rem;
  margin-top: 1rem;
  margin-bottom: 1rem;
}

.testimonials-link {
  display: flex;
  align-items: center;
  gap: 0.7rem;
  width: 10rem;
  font-weight: 400;
  font-size: 0.9rem;
  padding-bottom: 0.5rem;
}

.testimonials-content svg {
  transform: scale(1.6);
}

.testimonials-link:hover {
  border-bottom: 1px solid #fff;
}

@media (max-width: 425px) {
  .testimonials {
    display: block;
  }
}
</style>
