<template>
  <div class="container">
    <h1 className="repo-header">Repositories</h1>
    <div class="repo">
      <div class="repo-container">
        <h2>Carousel-review</h2>
        <p class="desc">Carousel-review react js</p>
        <div class="icon">
          <p class="id">ID:87979997</p>
          <i class="fa-solid fa-layer-group"></i>
        </div>
        <div class="lang-size">
          <p className="repo-lang"><i class="fa-regular fa-circle-dot"></i> React js</p>
          <p className="repo-size">140Kb</p>
        </div>
      </div>
      <div class="repo-container">
        <h2>Carousel-review</h2>
        <p class="desc">Carousel-review react js</p>
        <div class="icon">
          <p class="id">ID:87979997</p>
          <i class="fa-solid fa-layer-group"></i>
        </div>
        <div class="lang-size">
          <p className="repo-lang"><i class="fa-regular fa-circle-dot"></i> React js</p>
          <p className="repo-size">140Kb</p>
        </div>
      </div>
      <div class="repo-container">
        <h2>Carousel-review</h2>
        <p class="desc">Carousel-review react js</p>
        <div class="icon">
          <p class="id">ID:87979997</p>
          <i class="fa-solid fa-layer-group"></i>
        </div>
        <div class="lang-size">
          <p className="repo-lang"><i class="fa-regular fa-circle-dot"></i> React js</p>
          <p className="repo-size">140Kb</p>
        </div>
      </div>
      <div class="repo-container">
        <h2>Carousel-review</h2>
        <p class="desc">Carousel-review react js</p>
        <div class="icon">
          <p class="id">ID:87979997</p>
          <i class="fa-solid fa-layer-group"></i>
        </div>
        <div class="lang-size">
          <p className="repo-lang"><i class="fa-regular fa-circle-dot"></i> React js</p>
          <p className="repo-size">140Kb</p>
        </div>
      </div>
      <div class="repo-container">
        <h2>Carousel-review</h2>
        <p class="desc">Carousel-review react js</p>
        <div class="icon">
          <p class="id">ID:87979997</p>
          <i class="fa-solid fa-layer-group"></i>
        </div>
        <div class="lang-size">
          <p className="repo-lang"><i class="fa-regular fa-circle-dot"></i> React js</p>
          <p className="repo-size">140Kb</p>
        </div>
      </div>
      <div class="repo-container">
        <h2>Carousel-review</h2>
        <p class="desc">Carousel-review react js</p>
        <div class="icon">
          <p class="id">ID:87979997</p>
          <i class="fa-solid fa-layer-group"></i>
        </div>
        <div class="lang-size">
          <p className="repo-lang"><i class="fa-regular fa-circle-dot"></i> React js</p>
          <p className="repo-size">140Kb</p>
        </div>
      </div>
      <div class="repo-container">
        <h2>Carousel-review</h2>
        <p class="desc">Carousel-review react js</p>
        <div class="icon">
          <p class="id">ID:87979997</p>
          <i class="fa-solid fa-layer-group"></i>
        </div>
        <div class="lang-size">
          <p className="repo-lang"><i class="fa-regular fa-circle-dot"></i> React js</p>
          <p className="repo-size">140Kb</p>
        </div>
      </div>
      <div class="repo-container">
        <h2>Carousel-review</h2>
        <p class="desc">Carousel-review react js</p>
        <div class="icon">
          <p class="id">ID:87979997</p>
          <i class="fa-solid fa-layer-group"></i>
        </div>
        <div class="lang-size">
          <p className="repo-lang"><i class="fa-regular fa-circle-dot"></i> React js</p>
          <p className="repo-size">140Kb</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'RepoSection',
}
</script>

<style lang="scss" scoped>
@use 'sass:math';

/* variables*/
$primary: #4D73F8;
$base-gap: 30px;
$text-color: #020C18;
$background: #ffffff;

.container {
  margin: 30px 0;

  .repo-header {
    font-family: 'Merriweather';
    font-style: normal;
    font-weight: 700;
    font-size: 30px;
    color: $text-color;
  }

  .repo {
    padding: 20px;
    display: grid;
    gap: $base-gap;
    grid-template-columns: 1fr 1fr 1fr 1fr;

    .repo-container {
      box-sizing: border-box;
      background: #FFFFFF;
      border: 1px solid rgba(77, 115, 248, 0.15);
      border-radius: 6px;
      padding: $base-gap/2 $base-gap;

      h2 {
        color: $primary;
      }

      .desc {
        font-size: 16px;
      }

      .icon {
        display: flex;
        justify-content: space-between;
        align-items: center;

        .fa-layer-group {
          color: $primary;
        }

        .id {
          color: #616161;

        }
      }


      .lang-size {
        display: flex;
        justify-content: space-between;
        font-size: 15px;

        .fa-circle-dot {
          color: $primary;
        }
      }
    }
  }
}</style>