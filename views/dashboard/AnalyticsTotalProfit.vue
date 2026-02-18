<script setup lang="ts">
import { useTheme } from 'vuetify'

const vuetifyTheme = useTheme()

const currentTheme = computed(() => vuetifyTheme.current.value.colors)
</script>

<template>
  <VCard>
    <VCardItem>
      <VCardTitle>
        <VAvatar
          color="secondary"
          rounded
          size="40"
          class="elevation-2 avatar"
        >
          <VIcon
            size="24"
            icon="ri-pie-chart-2-line"
          />
        </VAvatar>
      </VCardTitle>

      <template #append>
        <div class="me-n3">
          <MoreBtn :menu-list="moreList" />
        </div>
      </template>
    </VCardItem>
    <VCardText class="ml-3 mt-1 mb-1">
      <VRow class="mb-1">
        <h4>Total Profit</h4>
      </VRow>
      <VRow>
        <h2>
          $25.6K
        </h2>
        <p class="text-success ml-3">+42%</p>
      </VRow>
      <VRow class="mt-1">
        <p>Weekly Project</p>
      </VRow>
    </VCardText>
  </VCard>
</template>

<style>
.avatar {
  border-radius: 50%;
}
</style>
