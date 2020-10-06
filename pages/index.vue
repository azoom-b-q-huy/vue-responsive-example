<template>
  <div class="container">
    <div class="new-item">
      <img
        class="img-responsive"
        src="https://d1o7cxaf8di5ts.cloudfront.net/file/media/origin/2020_03_04/9d878fccccecf3f3.jpg"
        alt="9d878fccccecf3f3.jpg"
      />
      <span style="font-size: 48px; font-weight: bold">AIR MAX VENORA</span>
      <br />
      <span class="description"
        >Classic sneaker remagined Carted Foam don't just make an impression,
        they make an impact.</span
      >
      <div class="shop">Shop</div>
    </div>
    <h2 class="title">Featured</h2>
    <div class="featured">
      <div class="item">
        <img
          class="img-responsive"
          src="https://lh3.googleusercontent.com/proxy/10L7g9J_fcXM3M4qBQLg8qgzJfh4R5D4d_nAte19QMxkjCBdmFWa7nITSqNrDnNoJFALDFjyLAFX2r5K4Bvu02fmwQXuTGZJbznJDyt7bMVI5PNeke-19I5KSjyVmfpXalTQpMZ8NDIS5tCaHtyfsJaVYj-wl-X2Xgp6lR5PZaGhMfL9_MI75C7ESvBh5TeJ-0Kw0rAZ91jAODGVUwWTq7wtwVT5DDIKOz_l7E0MQMBTKqlFxtbvYdbJaDMtyclJu5ni71Hr_CO-dVbL-izT21-GMJaID8PLI_Dmh2T1dhxCU55uLIyvLLCE"
          alt="9d878fccccecf3f3.jpg"
        />
        <div
          class="action"
          style="position: relative; bottom: 146px; left: 0px"
        >
          <div class="description"></div>
          <div>
            <div class="shop"></div>
            <div class="learn-more"></div>
          </div>
        </div>
      </div>
      <div class="divine"></div>
      <div class="item">
        <img
          class="img-responsive"
          src="https://lh3.googleusercontent.com/proxy/10L7g9J_fcXM3M4qBQLg8qgzJfh4R5D4d_nAte19QMxkjCBdmFWa7nITSqNrDnNoJFALDFjyLAFX2r5K4Bvu02fmwQXuTGZJbznJDyt7bMVI5PNeke-19I5KSjyVmfpXalTQpMZ8NDIS5tCaHtyfsJaVYj-wl-X2Xgp6lR5PZaGhMfL9_MI75C7ESvBh5TeJ-0Kw0rAZ91jAODGVUwWTq7wtwVT5DDIKOz_l7E0MQMBTKqlFxtbvYdbJaDMtyclJu5ni71Hr_CO-dVbL-izT21-GMJaID8PLI_Dmh2T1dhxCU55uLIyvLLCE"
          alt="9d878fccccecf3f3.jpg"
        />
      </div>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style lang="scss">
.container {
  padding: 0 48px;
  > .title {
    padding: 32px 0;
  }

  > .new-item {
    display: flex;
    flex-direction: column;
    align-items: center;

    > .description {
      text-align: center;
    }
    > .shop {
      background-color: black;
      color: white;
      padding: 8px 24px;
      border-radius: 24px;
      margin: 10px 0px;
    }
  }

  > .featured {
    display: flex;
    flex-direction: row;
    > .divine {
      width: 16px;
    }
    > .item {
      flex: 1;
    }
  }
}

.img-responsive {
  width: 100%;
  height: auto;
}

@media screen and (max-width: 600px) {
  .container {
    padding: 0 32px;
    > .new-item {
      align-items: flex-start;
      > .description {
        text-align: left;
      }
    }

    > .featured {
      flex-direction: column;
    }
  }
}
</style>
