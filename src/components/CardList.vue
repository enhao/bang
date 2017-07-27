<template>
  <div class="card-list">
    <div class="m-2">
      <b-form-input v-model="keyword" class="mb-2" type="text" placeholder="Search"></b-form-input>
      <div class="card-columns">
        <div v-for="card in filteredCards">
          <b-card :title="card.name.zh_tw" :sub-title="card.name.en_us" class="mb-2">
            {{ card.description }}
          </b-card>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import details from '../banginfo.json'

export default {
  name: 'card-list',
  data () {
    return {
      cards: [],
      keyword: ''
    }
  },
  mounted () {
    this.cards = details.playingCards
  },
  computed: {
    filteredCards: function () {
      let self = this
      return self.cards.filter(function (card) {
        let keyword = self.keyword.toLowerCase()
        return card.name.en_us.toLowerCase().indexOf(keyword) !== -1 ||
          card.name.zh_tw.toLowerCase().indexOf(keyword) !== -1
      })
    }
  }
}
</script>

<style>

</style>
