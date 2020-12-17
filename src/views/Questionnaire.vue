<template>
  <div class="open">
    <OpenEnded />
  </div>
</template>

<script>
// @ is an alias to /src
import OpenEnded from '@/components/OpenEnded.vue';

export default {
  name: 'Questionnaire',
  components: {
    OpenEnded,
  },
};
</script>
