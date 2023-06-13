<template>
  <Tutorial/>
</template>

<script>
export default {
  async asyncData(){
    const { data } = await $axio.get(
      'https:///i1ck4b91ex.microcms.io/api/vl/blog',
      {
        headers: { 'X-MICROCMS-API-KEY': 'iPAu3Flksctvva2qHappfJIramNmEQ2eEF2Z'}
      }
    )

    return data
  }
  
}
</script>
