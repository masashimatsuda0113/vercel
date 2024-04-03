<template>
    <div>
        <nav>
            <ul>
                <li><nuxt-link href="/">Home</nuxt-link></li>
                <li><nuxt-link href="/about">About</nuxt-link></li>
                <li><nuxt-link href="/special">special</nuxt-link></li>
            </ul>
        </nav>
        <slot />
    </div>
</template>

<style lang="scss" scoped>
nav {
  display: flex;
  justify-content: space-around;
  ul {
    list-style: none;
    padding: 0;
    margin: 0;
    display: flex;
    li {
      margin: 0 10px;
      a{
        text-decoration: none;
        color: #333;
        font-weight: bold;
        &.active {
          color: #0070f3;
        }
        &:hover {
          color: #0070f3;
        }
      }
    }
  }
}
</style>

