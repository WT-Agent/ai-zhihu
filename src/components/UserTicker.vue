<template>
  <div class="glass-card ticker-card">
    <div class="ticker-wrapper">
      <div v-for="(item, index) in tickerItems" :key="index" class="ticker-item">
        <span>{{ item.text }}</span>
        <span style="color: var(--success-color); font-weight: bold;">[生成完成]</span>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
import { ref } from 'vue';

const tickerItems = ref([
  {
    "text": "用户 138****3311 创作的社会热点回答斩获知乎 1W+ 赞同"
  },
  {
    "text": "用户 189****6622 获得了 AI 替代失业硬核科普回答大纲"
  },
  {
    "text": "用户 131****9900 完成了博弈论解构职场关系知乎体长文"
  },
  {
    "text": "用户 156****4455 生成了知乎盐选故事开场 Hook"
  },
  {
    "text": "用户 173****8811 取得了知乎想法引流与评论区控评 SOP"
  }
]);
</script>
