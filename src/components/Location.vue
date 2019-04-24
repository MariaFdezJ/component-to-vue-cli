<template>
  <div class="place" id="location">
    <img :src="img" width="235" height="300"/>
    <h2>{{ name[0].toUpperCase() + name.slice(1) }}</h2>
    <p>{{ desc }}</p>
  </div>
</template>

<script>
export default {
  name: 'Location',
  props: {
    name: {
      type: String,
      default: 'name of location'
    },
    img: {
      type: String,
      default: 'https://s3-us-west-2.amazonaws.com/s.cdpn.io/28963/moscow.svg'
    },
    desc: {
      type: String,
      default: 'Site\'s description'
    }
  }
}
</script>
