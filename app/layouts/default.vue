<template>
    <UContainer>
        <!-- Header (nav) -->
        <slot/>
        <!-- Footer -->
         <UFooter>
            <template #left>
                <p class="text-muted text-sm">Copyright Tim Mushen ©{{ new Date().getFullYear() }}</p>
            </template>

            <!-- Center Nav -->
            <UNavigationMenu :items="items" variant="link" />

            <template #right>
                <UButton 
                    icon="i-simple-icons-linkedin"
                    variant="outline"
                    color="neutral"
                    size="sm"
                    to="https://linkedin.com/in/timmushen"
                    target="_blank"
                />
            </template>
         </UFooter>
    </UContainer>
</template>
<script setup>
const items = [
    {
        label: "Home Page", 
        to: "/"
    },
    {
        label: "About", 
        to: "/about"
    },
    {
        label: "Portfolio", 
        to: "/portfolio"
    },
    {
        label: "Contact", 
        to: "/contact"
    },
]
</script>