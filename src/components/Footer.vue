<template>
  <div>
    <div class="top">
      <div class="container">
        <div class="row">
          <div class="col row">
            <div class="col">
              Lorem ipsum dolor sit amet consectetur adipisicing elit.
            </div>
            <div class="col">
              Lorem ipsum dolor sit amet consectetur adipisicing elit.
            </div>
            <div class="col">
              Lorem ipsum dolor sit amet consectetur adipisicing elit.
            </div>
            <div class="col">
              Lorem ipsum dolor sit amet consectetur adipisicing elit.
            </div>
          </div>
          <div class="col img"></div>
        </div>
      </div>
    </div>
    <div class="bottom">
      <div class="container">
        Lorem ipsum dolor sit, amet consectetur adipisicing elit. Cupiditate id
        obcaecati debitis optio quisquam, repudiandae eligendi. Ut molestiae
        laudantium officia, perspiciatis distinctio eaque, ducimus impedit enim
        voluptatibus eveniet perferendis deleniti.
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Footer",
};
</script>

<style scoped lang="scss">
@import "../scss/vars";

div {
  .top {
    color: $white-color;
    background-color: $grey-color;
    background-image: url("/images/footer-bg.jpg");

    .container {
      .row {
        display: flex;

        .row {
          width: 40%;
          display: flex;
          flex-wrap: wrap;

          .col {
            width: (100% / 3);
            padding: 0.8em;
          }
        }

        .img {
          flex-grow: 1;
          background-image: url("/images/dc-logo-bg.png");
          background-size: cover;
          background-repeat: no-repeat;
          background-position: center;
        }
      }
    }
  }

  .bottom {
    color: $white-color;
    background-color: $grey-color;
  }
}
</style>