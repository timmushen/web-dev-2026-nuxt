<template>
    <UFooter>
  <UNavigationMenu :items="items" variant="link" />
    </UFooter>
</template>
<script setup>
    const items = [
        {
            label: "Item 1",
            to: "/"
        },
        {
            label: "Item 2",
            to: "/"
        },
        {
            label: "Item 3", 
            to: "/"
        }
    ]
</script>