<script setup></script>

<template>
  <div>
    <div class="info-section">
      <div class="info-video">
        <video
          class="coffee-beans-video"
          autoplay
          loop
          muted
          playsinline
          webkit-playsinline
        >
          <source
            src="/src/assets/videos/2675509-hd_1920_1080_24fps.mp4"
            type="video/mp4"
          />
        </video>
      </div>
      <div class="info-text">
        <h2>Guatemalan Coffee: A Rich Tradition</h2>
        <p>
          From the renowned coffee-growing regions of Antigua and Huehuetenango
          in Guatemala, we procure beans known for their distinctive flavors and
          rich history. These high-altitude farms, often nestled between ancient
          volcanoes, benefit from mineral-rich soil and a unique microclimate,
          producing beans with vibrant acidity, full body, and notes of
          chocolate and citrus.
        </p>
        <h2>Colombian Coffee: The Heart of Excellence</h2>
        <p>
          In Colombia, our beans are sourced from the picturesque regions of
          Huila and Nariño. Colombian coffee is celebrated worldwide for its
          smooth, balanced flavor and bright acidity. The diverse landscape,
          ranging from mountainous terrains to lush rainforests, offers the
          perfect conditions for growing some of the most sought-after coffee
          beans. The result is a cup with hints of caramel, red fruits, and a
          floral aroma that captivates the senses.
        </p>
      </div>
    </div>
    <div class="info-section-2">
      <div class="info-text-2">
        <h2>Ethically Sourced Milk: Quality You Can Trust</h2>
        <p>
          We understand that the perfect cup of coffee isn't complete without
          the finest milk. We are committed to using ethically sourced milk from
          local farms that uphold the highest standards of animal welfare and
          environmental sustainability. Our dairy partners ensure their cows are
          pasture-raised, treated with care, and fed a natural diet, resulting
          in milk that is not only delicious but also ethically produced.
        </p>
        <h2>A Commitment to Sustainability and Fair Trade</h2>
        <p>
          We are proud to partner with farmers who practice sustainable and
          fair-trade farming methods. By working directly with these local
          farmers, we ensure that they receive fair compensation for their hard
          work, allowing them to invest in their communities and preserve the
          environment for future generations.
        </p>
      </div>
      <div class="info-video-2">
        <video
          class="cow-farm-video"
          autoplay
          loop
          muted
          playsinline
          webkit-playsinline
        >
          <source
            src="/src/assets/videos/4928679-uhd_4096_2160_25fps.mp4"
            type="video/mp4"
          />
        </video>
      </div>
    </div>
  </div>
</template>

<style scoped>
.info-section,
.info-section-2 {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  margin: 30px;
}

.info-text,
.info-text-2 {
  display: flex;
  flex-direction: column;
  gap: 50px;
  line-height: 1.7;
}

.info-section h2,
.info-section-2 h2 {
  background-color: #0e2a54;
  color: rgb(255, 229, 151);
  text-align: center;
  padding: 8px;
}

.coffee-beans-video,
.cow-farm-video {
  width: 100%;
  height: 400px;
  align-items: center;
  border-radius: 3px;
  overflow: hidden;
}

@media screen and (min-width: 1100px) {
  .info-section,
  .info-section-2 {
    flex-direction: row;
    gap: 60px;
    margin: 180px 120px;
  }
  .coffee-beans-video,
  .cow-farm-video {
    width: 500px;
  }
}
</style>
