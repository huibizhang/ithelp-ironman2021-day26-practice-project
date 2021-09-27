<template>
  <div :class="[
      'w-screen h-screen',
      'flex flex-col',
      'justify-center items-center',
      'gap-5',
    ]"
  >
    <RabbitButton />

    <RabbitButton text="wifi" color="blue">
      <template v-slot:iconLeft>
        <svg  xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M8.111 16.404a5.5 5.5 0 017.778 0M12 20h.01m-7.08-7.071c3.904-3.905 10.236-3.905 14.141 0M1.394 9.393c5.857-5.857 15.355-5.857 21.213 0" />
        </svg>
      </template>
    </RabbitButton>

    <div class="flex gap-5">
      <RabbitButton text="上一步" color="green">
      <template v-slot:iconLeft>
        <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M10 19l-7-7m0 0l7-7m-7 7h18" />
        </svg>
      </template>
    </RabbitButton>

    <RabbitButton text="下一步" color="green">
      <template v-slot:iconRight>
        <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M14 5l7 7m0 0l-7 7m7-7H3" />
        </svg>
      </template>
    </RabbitButton>
    </div>
  </div>
</template>

<script>
import RabbitButton from './components/RabbitButton.vue'

export default {
  data() {
    return {

    }
  },
  components: {
    RabbitButton,
  }
}
</script>