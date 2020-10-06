<template>
  <div class="layout">
    <div id="mobile-nav">
      <LogoIcon />
      <div class="menu">
        <div class="menu-item"><CartIcon /></div>
        <div class="menu-item"><SearchIcon /></div>
        <div class="menu-item"><MenuIcon /></div>
      </div>
    </div>

    <p id="sub-action">Help | Join Us | Sign In</p>
    <div id="desktop-nav">
      <LogoIcon />
      <div class="category">
        <div v-for="(menu, index) in menus" :key="index" class="category-item">
          <span class="title">{{ menu.title }}</span>
        </div>
      </div>
      <div class="menu">
        <!-- <div class="menu-item">
          <button>SEARCH</button>
          <input type="text" />
        </div> -->
        <div class="menu-item"><FavouriteIcon /></div>
        <div class="menu-item"><CartIcon /></div>
      </div>
    </div>
    <div>
      <Nuxt />
    </div>
  </div>
</template>
<script>
import LogoIcon from '~/components/Icons/Logo'
import MenuIcon from '~/components/Icons/Menu'
import SearchIcon from '~/components/Icons/Search'
import CartIcon from '~/components/Icons/Cart'
import FavouriteIcon from '~/components/Icons/Favourite'

export default {
  components: {
    LogoIcon,
    MenuIcon,
    SearchIcon,
    CartIcon,
    FavouriteIcon
  },
  data() {
    return {
      menus: [
        { title: 'Men' },
        { title: 'Women' },
        { title: 'Kids' },
        { title: 'Customize' },
        { title: 'Sale' },
        { title: 'SNKRS' }
      ]
    }
  }
}
</script>
<style lang="scss">
#mobile-nav {
  display: none;
}

#desktop-nav {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  padding: 12px 32px;
  > .category {
    display: flex;
    flex-direction: row;
  }
  > .category > .category-item {
    display: flex;
    justify-content: center;
  }
  > .category > .category-item > .title {
    padding: 12px;
    font-weight: bold;
  }
  > .category > .category-item > .title:hover {
    cursor: pointer;
    border-bottom: 2px solid black;
  }
}

.logo {
  align-self: center;
}

.menu {
  display: flex;
  flex-direction: row;
}
.menu > .menu-item {
  padding: 12px 0px 12px 12px;
  display: flex;
  justify-content: center;
  align-items: center;
}

#sub-action {
  text-align: end;
  padding: 10px 32px;
  font-size: 10px;
  font-weight: bold;
  background-color: #f5f5f5;
}

@media screen and (max-width: 1096px) {
  #mobile-nav {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    padding: 12px 32px;
  }
  #desktop-nav {
    display: none;
  }
  #sub-action {
    display: none;
  }
}
</style>
