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
          color="primary"
          rounded
          size="40"
          class="elevation-2 avatar"
        >
          <VIcon
            size="24"
            icon="ri-file-word-2-line"
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
        <h4>New Project</h4>
      </VRow>
      <VRow>
        <h2>
          862
        </h2>
        <p class="text-error ml-3">-18%</p>
      </VRow>
      <VRow class="mt-1">
        <p>Yearly Project</p>
      </VRow>
    </VCardText>
  </VCard>
</template>

<style>
.avatar {
  border-radius: 50%;
}
</style>
