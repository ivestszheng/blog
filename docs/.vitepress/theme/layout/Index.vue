<script setup lang="ts">
import { useData } from 'vitepress'
import DefaultTheme from 'vitepress/theme'
import Comment from '../components/Comment.vue';

const { page } = useData()
const { Layout } = DefaultTheme
</script>

<template>
  <Layout>
    <template #doc-after>
      <Comment :key="page.relativePath"></Comment>
    </template>
  </Layout>
</template>
