<template>
  <UApp>
 <Navbar/>
 <UMain>
  <UPageHero title="Here's our page" description="This is built in Tailwind and Nuxt">

  </UPageHero>
  <Products/>
  <section class="flex flex-row justify-between gap-4 max-w-6xl mx-auto">
    <Bucket title="Title Here" className="bg-green-500">
        <b>Lorem ipsum dolor sit amet consectetur</b> 
      
        adipisicing elit. Voluptates voluptatum dolore at consequuntur assumenda voluptas quod quibusdam, nihil saepe harum, atque labore odio ex eum eius nam ipsam? Eligendi, animi?
    </Bucket>
    <Bucket title="Column 2" className="bg-gray-600" />
    <Bucket>slot</Bucket>
 
  </section>
  </UMain>
  <Footer/>
</UApp>
</template>
