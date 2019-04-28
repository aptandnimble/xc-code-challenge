<template>
  <div id="app">
    <nav-bar></nav-bar>
    <carousel></carousel>
    <main-content></main-content>
	<cta-block></cta-block>
    <site-footer></site-footer>
  </div>
</template>

<script>

import NavBar from './components/nav'
import Carousel from './components/carousel'
import MainContent from './components/content'
import CtaBlock from './components/ctablock'
import SiteFooter from './components/footer'

export default {
  name: 'app',
  components: {
	NavBar,
    Carousel,
    MainContent,
	CtaBlock,
	SiteFooter
  }
}
</script>

<style>
@import './assets/main.scss';

</style>
