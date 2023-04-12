<template>
   <div>
     <button>
            {{buttonText.text}}
        </button>
    </div>
</template>

<script>
    export default {
        buttonText: {
            type: Object,
            required: true
        }
    }
</script>