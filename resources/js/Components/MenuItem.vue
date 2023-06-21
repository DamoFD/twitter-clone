<template>
    <div>

    </div>
</template>

<script setup>
import { toRefs } from 'vue';
import Home from 'vue-material-design-icons/Home.vue';
import Pound from 'vue-material-design-icons/Pound.vue';
import BellOutline from 'vue-material-design-icons/BellOutline.vue';
import EmailOutline from 'vue-material-design-icons/EmailOutline.vue';
import AccountOutline from 'vue-material-design-icons/AccountOutline.vue';

const props = defineProps({
    iconString: String,
})

const { iconString } = toRefs(props)

let icon = null

if (iconString.value === 'Home') icon = Home
if (iconString.value === 'Explore') icon = Pound
if (iconString.value === 'Notifications') icon = BellOutline
if (iconString.value === 'Messages') icon = EmailOutline
if (iconString.value === 'Profile') icon = AccountOutline
</script>

<style lang="scss" scoped>

</style>