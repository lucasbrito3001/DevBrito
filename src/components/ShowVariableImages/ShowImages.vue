<template>
  <ul id="list-stacks">
          <li class="item-stacks" v-for="tech in propsTechsToShow" :key="tech.name">
            <figure class="figure-stacks">
              <img class="img-stack" :src="tech.src" :alt="tech.alt">
              <figcaption> 
                <span>{{tech.name}}</span> 
                <span id="tech-level">{{tech.level}}</span> 
              </figcaption>
            </figure>
          </li>
        </ul>
</template>

<script>
export default {
    name: 'ShowImages',

    props: {
        propsTechsToShow: {
            type: Array
        }
    }
}
</script>

<style src='./showImages.scss' lang='scss' scoped/>