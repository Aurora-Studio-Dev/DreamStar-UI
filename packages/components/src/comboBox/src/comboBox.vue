<script setup lang="ts">
import { computed } from "vue";

defineOptions({
  name: "DsComboBox",
});

interface Prop {
  type: string;
}

const props = defineProps<Prop>();

const classList = computed(() => {
  const { type } = props;
  return {
    [`ea-button--${type}`]: type,
  };
});
</script>

<template>

</template>
