<script>
export default {
  name: "AppFirtstFooter",
};
</script>

<template>
  <div class="container">
    <!-- list 1 -->
    <div>
      <div class="footer-list">
        <h3>DC COMICS</h3>
        <ul>
          <li>
            <a href="#">Characters</a>
          </li>
          <li>
            <a href="#">Comics</a>
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
            <a href="#">Videos</a>
          </li>
          <li>
            <a href="#">News</a>
          </li>
        </ul>
      </div>
      <!-- list 2 -->
      <div class="footer-list">
        <h3>SHOP</h3>
        <ul>
          <li>
            <a href="#">Shop DC</a>
          </li>
          <li>
            <a href="#">Shop DC Collectibles</a>
          </li>
        </ul>
      </div>
    </div>
    <!-- list 3 -->
    <div class="footer-list">
      <h3>DC</h3>
      <ul>
        <li>
          <a href="#">Terms Of Use</a>
        </li>
        <li>
          <a href="#">Privacy policy (New)</a>
        </li>
        <li>
          <a href="#">Ad Choices</a>
        </li>
        <li>
          <a href="#">Advertising</a>
        </li>
        <li>
          <a href="#">Jobs</a>
        </li>
        <li>
          <a href="#">Subscription</a>
        </li>
        <li>
          <a href="#">Talent Workshops</a>
        </li>
        <li>
          <a href="#">CPSC Certificates</a>
        </li>
        <li>
          <a href="#">Ratings</a>
        </li>
        <li>
          <a href="#">Shop Help</a>
        </li>
        <li>
          <a href="#">Contact Us</a>
        </li>
      </ul>
    </div>
    <!-- lista 4 -->
    <div class="footer-list">
      <h3>SITES</h3>
      <ul>
        <li>
          <a href="#">DC</a>
        </li>
        <li>
          <a href="#">MAD Magazine</a>
        </li>
        <li>
          <a href="#">DC Kids</a>
        </li>
        <li>
          <a href="#">DC Universe</a>
        </li>
        <li>
          <a href="#">DC Power Visa</a>
        </li>
      </ul>
    </div>
  </div>
</template>

<style lang="scss" scoped>
@use "/src/styles/partial/mixins" as *;
@use "/src/styles/partial/variables" as *;

.container {
  display: flex;
  gap: 50px;
  padding: 50px 0;
  color: #fff;
  @include container90;
}

.footer-list {
  margin-bottom: 20px;
  h3 {
    margin-bottom: 10px;
  }

  ul {
    list-style: none;

    li {
      margin-bottom: 3px;
    }
  }

  a {
    color: rgb(143, 143, 143);
    font-size: 12px;
  }
}
</style>
