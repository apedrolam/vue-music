<template lang="pug">
li
    h2: a(:href="artist.url" target="_blank")
        p {{ artist.name }}
        img(:src="artist.image[2]['#text']")
</template>

<script>

export default {
    name: 'artist',
    props: [ 'artist' ]
}

</script>

<style lang="stylus" scoped>
li
    margin: 10px 0
    padding 0 5px
    flex-basis: 0
    align-self flex-end
</style>
