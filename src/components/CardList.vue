<template>
  <div class="card-list">
    <div class="m-2">
      <b-form-input class="mb-2" type="text" placeholder="Search"></b-form-input>
      <div class="card-columns">
        <b-card title="Bang!" sub-title="Bang!" class="mb-2">
          被「Bang!」攻擊的玩家需要以有「射失」效果的牌抵銷，或被扣除一點生命值，在沒有裝備和特殊能力指定距離下，玩家只可攻擊距離為1的對手。
        </b-card>
        <b-card title="射失" sub-title="Missed!" class="mb-2">
          被「Bang!」效果攻擊時用作抵銷「Bang!」。
        </b-card>
        <b-card title="啤酒" sub-title="Beer" class="mb-2">
          回復一點生命值，在失去最後一點生命值時也可以使用。在剩餘兩人時無效果。
        </b-card>
        <b-card title="驚嚎" sub-title="Cat Balou" class="mb-2">
          棄掉任何一位玩家的隨機一張手牌或者面前的任一張牌。
        </b-card>
        <b-card title="恐慌" sub-title="Panic!" class="mb-2">
          從離自己距離1的一位玩家手上隨機抽去或面前中抽去一張牌加入手牌。
        </b-card>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'card-list'
}
</script>

<style>

</style>
