<script lang="ts" setup>
import type { PropType } from 'vue'
import { ref } from 'vue'
import { ButtonTypes } from '~/server/api/types'
const props = defineProps({
  label: String,
  type: String as PropType<ButtonTypes>,
})
const type = ref(props.type ?? ButtonTypes.primary)
</script>

<template>
  <button w-full h-8 hover:invert-50 :class="type">
    <span>{{ props.label }}</span> <i v-if="type === ButtonTypes.tertiary" class="i-bi-chevron-right px-2 ml-3" />
  </button>
</template>

<style scoped>
.primary {
  background-color: black;
  color: white;
}
.secondary {
  background-color: white;
  color: black;
  border: 1px solid black;
}
.tertiary span{
  font-family: Tous, Tous-fallback;
  letter-spacing: 2pt;
  font-size: 12px;
}
.tertiary {
  background-color: transparent;
  color: black;
}
</style>
