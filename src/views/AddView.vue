<template>
  <div class="lg:mx-auto w-full lg:max-w-7xl p-4">
    <div>
      <div class="md:grid md:grid-cols-3">
        <div>
          <div class="flex flex-col justify-center items-center">
            <div
              class="bg-red-50 w-[200px] h-[200px] rounded-full bg-[url('/svg/img_placeholder.svg')] bg-no-repeat bg-center">
              <img src="" alt="">
            </div>
            <div class="my-4">
              <button class="text-red-500 font-semibold py-2 px-4 hover:bg-red-50 transition-all rounded-md">Tambah Image</button>
            </div>
          </div>
        </div>
        <div class="md:col-span-2">
          <div class="border shadow-md p-5 rounded-xl">
            <div class="mb-2">
              <h2 class="text-red-500 font-semibold text-lg">Informasi Umum</h2>
            </div>

            <div class="mb-1">
              <div class="my-1">
                <span class="text-gray-600">Nomor</span>
              </div>
              <div class="my-1">
                <span class="font-semibold">#16</span>
              </div>
            </div>
            <div class="mb-1">
              <div class="my-1">
                <span class="text-gray-600">Nama</span>
              </div>
              <div class="my-1">
                <input type="text"
                  class="hover:bg-opacity-50 transition-all focus:ring-2 ring-red-400 outline-none border px-2 py-2 rounded-md bg-red-50 w-full caret-red-500">
              </div>
            </div>
            <div class="mb-1">
              <div class="my-1">
                <span class="text-gray-600">Nama</span>
              </div>
              <div class="my-1">
                <div
                  class="hover:bg-opacity-50 transition-all focus:ring-2 ring-red-400 outline-none border px-2 py-2 rounded-md bg-red-50 w-full caret-red-500">
                  <div class="flex">
                    <div class="flex-1"></div>
                    <div class="text-red-500">
                      <i class="bi bi-chevron-down"></i>
                    </div>
                  </div>
                </div>
              </div>
            </div>
            <div class="mb-1">
              <div class="my-1">
                <span class="text-gray-600">Classification</span>
              </div>
              <div class="my-1">
                <div
                  class="hover:bg-opacity-50 transition-all focus:ring-2 ring-red-400 outline-none border px-2 py-2 rounded-md bg-red-50 w-full caret-red-500">
                  <div class="flex">
                    <div class="flex-1"></div>
                    <div class="text-red-500">
                      <i class="bi bi-chevron-down"></i>
                    </div>
                  </div>
                </div>
              </div>
            </div>
            <div class="mb-1">
              <div class="my-1">
                <span class="text-gray-600">Recistant</span>
              </div>
              <div class="my-1">
                <div
                  class="hover:bg-opacity-50 transition-all focus:ring-2 ring-red-400 outline-none border px-2 py-2 rounded-md bg-red-50 w-full caret-red-500">
                  <div class="flex">
                    <div class="flex-1"></div>
                    <div class="text-red-500">
                      <i class="bi bi-chevron-down"></i>
                    </div>
                  </div>
                </div>
              </div>
            </div>

          </div>
          <div class="border shadow-md p-5 rounded-xl mt-4">
            <div class="mb-2">
              <h2 class="text-red-500 font-semibold text-lg">Evolution</h2>
            </div>
            <div>
              <button class="transition-all w-full p-2 bg-red-500 hover:bg-red-400 rounded-md text-white">
                <i class="bi bi-plus"></i>
                Tambah
              </button>
            </div>
          </div>
          <div class="p-5 mt-4">
            <div class="mb-2 flex justify-end">
              <button class="transition-all py-2 px-4 rounded-md border me-2 border-red-500 hover:bg-red-100 text-red-500">
                Batal
              </button>
              <button class="transition-all py-2 px-4 rounded-md bg-red-500 hover:bg-red-400 text-white">
                Tambah
              </button>
            </div>
          </div>
        </div>

      </div>
    </div>
  </div>
</template>

<script>
import { onMounted } from "vue";
import types from "@/data/types"

export default {
  data() {
    return {
      types
    }
  },
  setup(props, context) {
    onMounted(() => {
      try {
        context.emit("id-menu", 2)
      } catch (error) {
        console.log(error)
      }
    })
  }
}
</script>
@/data/types