<template>
    <div>
        <p v-if="canSee">You can see this!</p>
        <p v-else>You cannot see this...</p>
    </div>
</template>

<script>
export default {
    name: "ShowHide",
    props: {
        canSee: Boolean,
    }
}
</script>