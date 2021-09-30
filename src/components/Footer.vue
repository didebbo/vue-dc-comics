<template>
  <footer>
    <div class="top">
      <div class="container">
        <div class="row">
          <div class="col row">
            <div class="col">
              <div class="title">Dc Comics</div>
              <ul>
                <li>
                  <a href="#">Characters</a>
                </li>
                <li>
                  <a href="#">Movies</a>
                </li>
                <li>
                  <a href="#">TV</a>
                </li>
                <li>
                  <a href="#">Games</a>
                </li>
                <li>
                  <a href="#">Video</a>
                </li>
                <li>
                  <a href="#">News</a>
                </li>
              </ul>
            </div>
            <div class="col">
              <div class="title">Dc Comics</div>
              <ul>
                <li>
                  <a href="#">Characters</a>
                </li>
                <li>
                  <a href="#">Movies</a>
                </li>
                <li>
                  <a href="#">TV</a>
                </li>
                <li>
                  <a href="#">Games</a>
                </li>
                <li>
                  <a href="#">Video</a>
                </li>
                <li>
                  <a href="#">News</a>
                </li>
              </ul>
            </div>
            <div class="col">
              <div class="title">Dc Comics</div>
              <ul>
                <li>
                  <a href="#">Characters</a>
                </li>
                <li>
                  <a href="#">Movies</a>
                </li>
                <li>
                  <a href="#">TV</a>
                </li>
                <li>
                  <a href="#">Games</a>
                </li>
                <li>
                  <a href="#">Video</a>
                </li>
                <li>
                  <a href="#">News</a>
                </li>
              </ul>
            </div>
            <div class="col">
              <div class="title">Dc Comics</div>
              <ul>
                <li>
                  <a href="#">Characters</a>
                </li>
                <li>
                  <a href="#">Movies</a>
                </li>
                <li>
                  <a href="#">TV</a>
                </li>
                <li>
                  <a href="#">Games</a>
                </li>
                <li>
                  <a href="#">Video</a>
                </li>
                <li>
                  <a href="#">News</a>
                </li>
              </ul>
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
  </footer>
</template>

<script>
export default {
  name: "Footer",
};
</script>

<style scoped lang="scss">
@import "../scss/vars";

footer {
  .top {
    color: $white-color;
    background-color: $grey-color;
    background-image: url("/images/footer-bg.jpg");

    .container {
      > .row {
        display: flex;

        .row {
          display: flex;
          flex-wrap: wrap;
          padding: 1em 0;

          .col {
            width: (100% / 3);
            padding: 0.8em;

            .title {
              font-weight: bold;
              font-size: 1.2em;
            }

            ul {
              li {
                a {
                  text-decoration: none;
                  color: $white-color;
                  opacity: 0.6;
                  text-transform: none;
                }
              }
            }
          }
        }

        .img {
          margin: 0 10em;
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