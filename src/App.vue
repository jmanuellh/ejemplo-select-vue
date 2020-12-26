<template>
  <div>
    <header>
      <h1>
        Ejemplo select vue
      </h1>      
    </header>
    <main>
      <section>
        <article>
          <h2>Seleccion</h2>
          <select v-model="selected">
            <option>Uno</option>
            <option>Dos</option>
            <option>Tres</option>
          </select>
        </article>
        <article>
          <h2>Seleccion de objectos</h2>
          <select v-model="selectedObject">
            <option v-bind:value="{nombre: 'uno', numero: 1}">Uno</option>
            <option v-bind:value="{nombre: 'dos', numero: 2}">Dos</option>
            <option v-bind:value="{nombre: 'tres', numero: 3}">Tres</option>
          </select>
        </article>
      </section>
    </main>
  </div>
</template>

<script>

export default {
  name: 'App',
  data() {
    return {
      selected: '',
      selectedObject: {
        nombre: '',
        numero: 0
      },
    }
  }
}
</script>

<style>
</style>
