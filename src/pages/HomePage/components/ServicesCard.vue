<template>
    <div class="card border border-light-gray rounded-lg p-5 flex  items-center gap-3">
        <div class="icon">
            <slot name="icon" />
        </div>
        <div class="text">
            <slot name="text" />
        </div>
    </div>
</template>
<script>
export default {

}
</script>