<script setup lang="ts">
import { useI18n } from 'vue-i18n'
import { useRouter } from 'vue-router'

const { t } = useI18n()

const router = useRouter()

router.replace({ query: { baz: 'bim' } })
</script>

<template>
  <div>
    {{ t('not-found') }}
  </div>
</template>

<route lang="yaml">
meta:
  layout: 404
</route>
