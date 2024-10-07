<template>
  <div class="flex items-start gap-3">
    <div>
      <UIcon :name="icon" />
    </div>

    <div class="flex flex-col">
      <h3 class="text-lg font-semibold">
        <ContentSlot :name="title" />
      </h3>
      <span>
        <ContentSlot :name="description" />
      </span>
    </div>
  </div>
</template>

<script setup lang="ts">
defineProps({
  icon: {
    type: String,
    default: "i-ph-cursor-click",
  },
});
</script>
