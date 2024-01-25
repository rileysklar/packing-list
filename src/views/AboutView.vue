<script>
export default {
  methods: {
    visitPortfolio() {
      window.open("https://rileysklar.io", "_blank");
    },
  },
};
</script>
<template>
  <div class="about">
    <h1>👋 Hi, I'm Riley</h1>
    <div class="content-section">
      <div>
        Hi, I’m Riley. I’m an innovative Full Stack Developer from Austin, TX
        with a proficiency in UI/UX Design. I manage a team of designers and
        developers to prototype, design, and develop integrated web applications
        for a variety of clients including Fortune 500 companies, multi-billion
        dollar lighting manufacturers, and state government agencies.
      </div>

      <div>
        Using tools such as JavasScript, Tailwind CSS, React, Astro, jQuery,
        Supabase, WP Engine, AWS, GitHub, WordPress and Figma, my team and I
        have a knack for creating exceptional online experiences. I’m on a
        mission to optimize the design to development workflow. Let’s
        collaborate and craft digital wonders that leave a lasting impression!
        🚀💻 Click the link in my contact bubble to visit my portfolio 🔗
      </div>
    </div>
    <button @click="visitPortfolio">Visit My Portfolio</button>
  </div>
</template>

<style>
.about {
  display: flex;
  flex-direction: column;
  max-width: 500px;
  width: 100%;
  margin: 0 auto;
  padding: 40px 16px;
  gap: 20px;
}
h1 {
  text-align: center;
}

.content-section {
  display: flex;
  flex-direction: column;
  gap: 20px;
}

button {
  background-color: white;
  color: black;
  padding: 12px 24px;
  border-radius: 100px;
  transition: all ease 0.2s;
}

button:hover {
  transform: scale(1.02);
  background-color: #41b080;
}

button:active {
  transform: scale(0.98);
}
</style>
