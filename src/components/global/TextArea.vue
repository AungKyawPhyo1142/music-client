<template>
    <label 
        for=""
        class="
            block
            uppercase
            tracking-wide
            text-gray-900
            text-xs
            font-bold
            mb-2
        "
        >
        {{ label }}
    </label>
    <textarea 
    class="
        appearance-none 
        block 
        w-full 
        bg-white 
        text-gray-700 
        border 
        border-gray-400 
        rounded 
        py-3 
        px-4 
        leading-tight 
        focus:outline-none 
        focus:bg-white 
        focus:border-gray-500
        " 
    v-model="descriptionComputed" cols="30" rows="10" :placeholder="placeholder"></textarea>
    <span class="text-red-500" v-if="error">
    {{ error }}</span>
</template>


<script setup>
    import { computed, defineProps, defineEmits,toRefs } from 'vue';

    const emit = defineEmits(['update:description'])

    const props = defineProps({
        label: String,
        description: String,
        placeholder: {type:String, default: ''},
        error: String
    });

    const {label, description, placeholder, error } = toRefs(props);

    const descriptionComputed = computed({
        get: ()=> description.value,
        set: (val) => emit('update:description',val)

    })


</script>

