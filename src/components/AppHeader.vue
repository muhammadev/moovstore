<template>
  <div class="header">
    <TopHeader />
    <MidHeader />
    <BtmHeader />
  </div>
</template>

<script>
import TopHeader from "../components/headerComponents/TopHeader";
import MidHeader from "../components/headerComponents/MidHeader";
import BtmHeader from "../components/headerComponents/BtmHeader";

export default {
  name: "HelloWorld",
  components: {
    TopHeader,
    MidHeader,
    BtmHeader
  }
};
</script>
