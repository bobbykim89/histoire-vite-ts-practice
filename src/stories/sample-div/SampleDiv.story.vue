<script setup lang="ts">
import SampleDiv from '../../components/sample-div'
import { ref } from 'vue'
// import { hstEvent } from 'histoire/client';

const text = ref('default text')
</script>

<docs lang="md">
# Title

## Sub title

- first
- second
- third
</docs>

<template>
  <Story title="Sample Div">
    <SampleDiv> {{ text }} </SampleDiv>

    <template #controls>
      <HstText v-model="text" title="default slot"> </HstText>
    </template>
  </Story>
</template>
