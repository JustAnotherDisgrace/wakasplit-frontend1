<template>
  <div class="small">
    <Card>
      <template #header>
        <img alt="user header" src="https://i.imgur.com/WoQhP7g.png">
      </template>
      <template #title>
        Advanced Card
      </template>
      <template #content>
        Lorem ipsum dolor sit amet, consectetur adipisicing elit. Inventore sed
        consequuntur error repudiandae numquam deserunt quisquam repellat libero
        asperiores earum nam nobis, culpa ratione quam perferendis esse,
        cupiditate neque quas!
      </template>
      <template #footer>
        <Button icon="pi pi-check" label="Save" @click="banana()" />
        <Button
          icon="pi pi-times"
          label="Cancel"
          class="p-button-secondary"
          style="margin-left: 0.5em"
        />
      </template>
    </Card>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
import Card from 'primevue/card/Card'
import Button from 'primevue/button/Button'

export default Vue.extend({
  name: 'IndexPage',
  components: { Card, Button },
  methods: {
    banana () {
      alert('Hello There')
    }
  }
})
</script>

<style>
.small {
  max-width: 450px;
}
</style>
