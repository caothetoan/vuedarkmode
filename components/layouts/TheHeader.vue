<!-- *************************************************************************
     TEMPLATE
     ************************************************************************* -->

<template lang="pug">
header.c-the-header
  the-logo

  base-divider

  base-heading(
    type="h1"
  ) A MINIMALIST DARK DESIGN SYSTEM FOR VUE.JS 👩‍🎨👨‍🎨

  base-heading(
    color="grey"
    fontWeight="regular"
    type="h2"
  ) Based components for the insomniacs who enjoy dark interfaces as much as we do.

  the-github-buttons(
    class="c-the-header__github-buttons"
    repo="vuedarkmode"
    user="lecoupa"
  )
  the-subscription-box
</template>

<!-- *************************************************************************
     SCRIPT
     ************************************************************************* -->

<script>
// PROJECT
import BaseDivider from "@/components/darkmode/base/BaseDivider";
import BaseHeading from "@/components/darkmode/base/BaseHeading";
import TheGithubButtons from "@/components/layouts/TheGithubButtons";
import TheLogo from "@/components/layouts/TheLogo";
import TheSubscriptionBox from "@/components/layouts/TheSubscriptionBox";

export default {
  components: {
    BaseDivider,
    BaseHeading,
    TheGithubButtons,
    TheLogo,
    TheSubscriptionBox
  }
};
</script>

<!-- *************************************************************************
     STYLE
     ************************************************************************* -->

<style lang="scss">
$c: ".c-the-header";

#{$c} {
  #{$c}__github-buttons {
    margin-top: 20px;
  }
}
</style>
