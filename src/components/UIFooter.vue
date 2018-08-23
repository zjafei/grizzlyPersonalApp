<template>
    <BottomNav
      slot="footer"
      class="bottomNav"
      @change="changeIteam"
    >
    <BottomNavItem value="首页" title="首页" icon=":icon-home"></BottomNavItem>
    <BottomNavItem value="熊论" title="熊论" icon=":icon-flag"></BottomNavItem>
    <BottomNavItem value="实习" title="实习" icon=":icon-rocket1"></BottomNavItem>
    <BottomNavItem value="我的" title="我的" icon=":icon-user"></BottomNavItem>
  </BottomNav>
</template>

<script>
import { BottomNav } from 'muse-ui';
import { BottomNavItem } from 'muse-ui/lib/BottomNav';
export default {

  components: {
    BottomNav,
    BottomNavItem
  },
  methods: {
    changeIteam (value) {
      console.log(value);
    }
  },
  mounted () { }
};
</script>
<style lang="less" scoped>
.bottomNav{
  background-color:  #fff;
  color:#fff;
  height: 50px;
  // {
  //   color:#fff;
  // }
}
</style>
