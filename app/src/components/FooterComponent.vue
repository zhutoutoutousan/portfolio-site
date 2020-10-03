<template>
  <footer class="footer">
      <div class="footer__item">
          &copy; 2020 Tian Shao. All Rights Reserved.
      </div>
      <div class="footer__item">
          <div class="footer__contact"><a href="mailto:stupidpieceofshit@126.com" class="footer__link">stupidpieceofshit@126.com |</a></div>
          <div class="footer__contact"><a href="tel: +8618852729551" class="footer__link"> | +8618852729551</a></div>
      </div>
  </footer>
</template>

<script>
export default {

}
</script>

<style lang="scss" scope>

.footer {
    position: absolute;
    bottom: 0;
    left: 0;
    width: 100%;
    padding: 3rem;
    background: $color-footer;
    color: $color-text;
    font-size: 1.6rem;
    text-align: center;
    font-family: $font-secondary;
    border-top: 1px solid $color-primary;
    user-select: text;
    overflow: hidden;

    &__item {
        display: inline-block;
        &:not(:last-child) {margin-right: 8rem;}

        @media only screen and (max-width: 50em) {
            display: block;
            &:not(:last-child) {
                margin-right: 0;
                margin-bottom: 1rem;
            }
            text-align: left;
        }
    }

    &__contact {
        display: inline-block;
        &:not(:not-child) {margin-right: 3rem;}

        @media only screen and (max-width: 50em) {
            &:not(:last-child) {
                margin-right: 3rem;
                margin-bottom: .5rem;
            }
        }
    }

    &__link {
        &:link, &:visited {
            color: $color-white;
            text-decoration: none;
        }
    }
}


</style>>
