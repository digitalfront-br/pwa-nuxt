<template>
  <header class="uk-background-muted">
    <div class="uk-container">
    <nav class="uk-navbar menu-topo" uk-navbar="">
      <div class="uk-navbar-left">
        <nuxt-link class=" uk-padding-small uk-padding-remove-horizontal logo" to="/">
          <img class="desktop uk-visible@m" src="@/assets/img/logo.svg" alt="" />
          <img class="mobile uk-padding uk-padding-remove-vertical uk-hidden@m" src="@/assets/img/logo.svg" alt="" />
        </nuxt-link>
      </div>
      <div class="uk-navbar-right">
          <ul class="uk-navbar-nav uk-visible@m">
            <li><nuxt-link to="/">item aqui</nuxt-link></li>
            <li><nuxt-link to="/">item aqui</nuxt-link></li>
            <li><nuxt-link to="/">item aqui</nuxt-link></li>
          </ul>
          <a
            href="#mobile-menu"
            class="uk-padding uk-padding-remove-vertical uk-hidden@m" uk-icon="icon: menu; ratio: 1.3"
            uk-toggle=""></a>
      </div>
    </nav>
    </div>
  </header>
</template>
