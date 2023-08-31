<template>
  <div class="lg:mx-auto w-full lg:max-w-7xl">
    <div>
      <div class="flex flex-wrap justify-center">

        <div class="rounded-xl shadow-md p-4 bg-white border m-4">
          <div class="font-semibold text-gray-500">
            <span>#1</span>
          </div>
          <div class="p-2 w-[200px]">
            <img src="/img/bulbasaur.jpeg" alt="">
          </div>
          <div class="py-2">
            <h2 class="text-center text-red-500 font-semibold text-lg">Bulbasaur</h2>
          </div>
          <div class="px-2 flex flex-wrap items-center justify-center">
            <button class="bg-[#78C850] hover:bg-opacity-80 py-1 px-2 text-white rounded-md m-1 transition-all">
              Grass
            </button>
            <button class="bg-[#A040A0] hover:bg-opacity-80 py-1 px-2 text-white rounded-md m-1 transition-all">
              Poison
            </button>
          </div>
        </div>
        <div class="rounded-xl shadow-md p-4 bg-white border m-4">
          <div class="font-semibold text-gray-500">
            <span>#1</span>
          </div>
          <div class="p-2 w-[200px]">
            <img src="/img/bulbasaur.jpeg" alt="">
          </div>
          <div class="py-2">
            <h2 class="text-center text-red-500 font-semibold text-lg">Bulbasaur</h2>
          </div>
          <div class="px-2 flex flex-wrap items-center justify-center">
            <button class="bg-[#78C850] hover:bg-opacity-80 py-1 px-2 text-white rounded-md m-1 transition-all">
              Grass
            </button>
            <button class="bg-[#A040A0] hover:bg-opacity-80 py-1 px-2 text-white rounded-md m-1 transition-all">
              Poison
            </button>
          </div>
        </div>
        <div class="rounded-xl shadow-md p-4 bg-white border m-4">
          <div class="font-semibold text-gray-500">
            <span>#1</span>
          </div>
          <div class="p-2 w-[200px]">
            <img src="/img/bulbasaur.jpeg" alt="">
          </div>
          <div class="py-2">
            <h2 class="text-center text-red-500 font-semibold text-lg">Bulbasaur</h2>
          </div>
          <div class="px-2 flex flex-wrap items-center justify-center">
            <button class="bg-[#78C850] hover:bg-opacity-80 py-1 px-2 text-white rounded-md m-1 transition-all">
              Grass
            </button>
            <button class="bg-[#A040A0] hover:bg-opacity-80 py-1 px-2 text-white rounded-md m-1 transition-all">
              Poison
            </button>
          </div>
        </div>
        <div class="rounded-xl shadow-md p-4 bg-white border m-4">
          <div class="font-semibold text-gray-500">
            <span>#1</span>
          </div>
          <div class="p-2 w-[200px]">
            <img src="/img/bulbasaur.jpeg" alt="">
          </div>
          <div class="py-2">
            <h2 class="text-center text-red-500 font-semibold text-lg">Bulbasaur</h2>
          </div>
          <div class="px-2 flex flex-wrap items-center justify-center">
            <button class="bg-[#78C850] hover:bg-opacity-80 py-1 px-2 text-white rounded-md m-1 transition-all">
              Grass
            </button>
            <button class="bg-[#A040A0] hover:bg-opacity-80 py-1 px-2 text-white rounded-md m-1 transition-all">
              Poison
            </button>
          </div>
        </div>
        <div class="rounded-xl shadow-md p-4 bg-white border m-4">
          <div class="font-semibold text-gray-500">
            <span>#1</span>
          </div>
          <div class="p-2 w-[200px]">
            <img src="/img/bulbasaur.jpeg" alt="">
          </div>
          <div class="py-2">
            <h2 class="text-center text-red-500 font-semibold text-lg">Bulbasaur</h2>
          </div>
          <div class="px-2 flex flex-wrap items-center justify-center">
            <button class="bg-[#78C850] hover:bg-opacity-80 py-1 px-2 text-white rounded-md m-1 transition-all">
              Grass
            </button>
            <button class="bg-[#A040A0] hover:bg-opacity-80 py-1 px-2 text-white rounded-md m-1 transition-all">
              Poison
            </button>
          </div>
        </div>

      </div>
    </div>
  </div>
</template>

<script>
import { onMounted } from "vue";

export default {
  setup(props, context) {
        onMounted(() => {
            try {
                context.emit("id-menu", 1)
            } catch (error) {
                console.log(error)
            }
        })
    }
}
</script>
