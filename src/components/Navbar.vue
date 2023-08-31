<template>
    <div>
        <nav class="bg-red-500">
            <div class="max-w-screen-xl flex flex-wrap items-center justify-between mx-auto p-4">
                <div class="flex items-center" v-if="rl[1]">
                    <img src="/pokemon.svg" class="h-8 mr-3" alt="Pokemon Logo" />
                    <span class="self-center text-2xl font-semibold whitespace-nowrap dark:text-white"></span>
                </div>

                <button v-if="rl[2]" @click="$router.push('/')" class="flex items-center text-white transition-all hover:bg-white hover:bg-opacity-20 active:bg-opacity-30 p-2 rounded-lg">
                    <i class="bi bi-chevron-left"></i>
                    <span class="px-2 self-center font-semibold whitespace-nowrap">
                        Tambah Baru
                    </span>
                </button>

                <div class="text-white text-lg">
                    <button v-if="rl[3]" class="rounded-full hover:bg-gray-50 hover:bg-opacity-25 active:bg-opacity-40 transition-all px-3 py-2">
                        <i class="bi bi-three-dots-vertical"></i>
                    </button>
                    <button @click="$router.push('/add')" v-if="rl[1]" class="rounded-full hover:bg-gray-50 hover:bg-opacity-25 active:bg-opacity-40 transition-all px-3 py-2">
                        <i class="bi bi-plus-lg"></i>
                    </button>
                </div>
            </div>
        </nav>
    </div>
    <!-- {{ rl }} -->
</template>

<script>
import { ref } from "vue";

export default {
    props: {
        idMenu: Number
    },
    setup(props) {
        const rl = ref([
            false,
            false,
            false,
            false
        ]);
        if (props.idMenu == 0) {
            rl.value[0] = true;
        }
        if (props.idMenu == 1) {
            rl.value[1] = true;
        }
        if (props.idMenu == 2) {
            rl.value[2] = true;
        }
        if (props.idMenu == 3) {
            rl.value[3] = true;
        }

        return {
            rl
        }
    }
}
</script>