

<template>
  <div class="h-screen bg-gray-100">
  <!-- Header -->
  <header class="flex justify-center py-4">
    <h1 class="text-3xl font-bold">Shop en ligne</h1>
  </header>

  <!-- Navigation -->
  <nav class="flex justify-center py-2">
  <ul class="flex justify-center">
    <li class="mr-4">
      <a href="#" class="text-gray-600 hover:text-gray-900">
        <i class="fas fa-home"></i> Accueil
      </a>
    </li>
    <li class="mr-4">
      <a href="#" class="text-gray-600 hover:text-gray-900">
        <i class="fas fa-shopping-bag"></i> Produits
      </a>
    </li>
    <li class="mr-4">
      <a href="#" class="text-gray-600 hover:text-gray-900">
        <i class="fas fa-cart-plus"></i> Panier
      </a>
    </li>
  </ul>
</nav>

  <!-- Featured products -->
  
  <section class="py-12">
    <h2 class="text-2xl font-bold mb-4">Produits en vedette</h2>
    <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-4">
      <div class="bg-white shadow-md rounded p-4">
        <img src="../assets/robe.jpg" alt="Product image" class="w-full h-48 object-cover rounded-t">
        <h3 class="text-lg font-bold">Robe</h3>
        <p class="text-gray-600">Lorem Ipsum is simply dummy text of the printing and typesetting industry. </p>
        <button class="bg-orange-500 hover:bg-orange-700 text-white font-bold py-2 px-4 rounded">Ajouter au panier</button>
      </div>
      <div class="bg-white shadow-md rounded p-4">
        <img src="../assets/robe.jpg" alt="Product image" class="w-full h-48 object-cover rounded-t">
        <h3 class="text-lg font-bold">Pantallon</h3>
        <p class="text-gray-600">Lorem Ipsum is simply dummy text of the printing and typesetting industry.</p>
        <button class="bg-orange-500 hover:bg-orange-700 text-white font-bold py-2 px-4 rounded">Ajouter au panier</button>
      </div>
      <div class="bg-white shadow-md rounded p-4">
        <img src="../assets/robe.jpg" alt="Product image" class="w-full h-48 object-cover rounded-t">
        <h3 class="text-lg font-bold">Jupe</h3>
        <p class="text-gray-600">Lorem Ipsum is simply dummy text of the printing and typesetting industry.</p>
        <button class="bg-orange-500 hover:bg-orange-700 text-white font-bold py-2 px-4 rounded">Ajouter au panier</button>
      </div>
    </div>
  </section>

  <!-- Call to action -->
  <section class="py-12">
    <h2 class="text-2xl font-bold mb-4">Découvrez nos produits</h2>
    <button class="bg-orange-500 hover:bg-orange-700 text-white font-bold py-2 px-4 rounded">Voir tous les produits</button>
  </section>

  <!-- Footer -->
  <footer class="py-4">
    <p class="text-gray-600">Copyright 2023 Shop en ligne</p>
  </footer>
</div>
</template>
<script>
export default {
  name: 'HomePage',

  methods: {
    addToCart(product) {
      // Ajouter le produit au panier
      console.log(`Ajout du produit ${product.name} au panier`)
    },
    goToProducts() {
      // Redirection vers la page des produits
      console.log('Redirection vers la page des produits')
    }
  }
}
</script>

<style>

</style>