<template>
  <div class="hello">
    <ul>
      <li v-for="item in info" :key="item.id">{{ item.title }}</li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    msg: String
  },
  data() {
    return {
      info: null
    };
  },
  mounted() {
    this.info = [
      {
        id: 1,
        star: 1,
        faktor: 1,
        title: "Simpel, fehlerfrei",
        description: "(Blog-Texte, Produktbeschreibungen etc.)",
        created_at: null,
        updated_at: "2018-01-06 17:39:53",
        selected: null
      },
      {
        id: 2,
        star: 2,
        faktor: 1.7,
        title: "Fehlerfrei & Recherchiert",
        description: "(Webseitentexte, Bewerbung etc.)",
        created_at: null,
        updated_at: "2018-01-06 17:40:25",
        selected: null
      },
      {
        id: 3,
        star: 3,
        faktor: 2.4,
        title: "Fachlich recherchiert",
        description: "(Pressetexte, Biografie etc.)",
        created_at: null,
        updated_at: "2018-01-09 05:14:25",
        selected: 1
      },
      {
        id: 4,
        star: 4,
        faktor: 3.1,
        title: "Wissenschaftlich & Recherchiert",
        description: "(Bachelorarbeit, Diplom etc.)",
        created_at: null,
        updated_at: "2018-01-06 17:41:00",
        selected: null
      },
      {
        id: 5,
        star: 5,
        faktor: 3.8,
        title: "Ausgearbeitet mit Konzept",
        description: "(z.B. Skript, Doktorarbeit, Rede etc.)",
        created_at: null,
        updated_at: "2018-01-06 17:41:22",
        selected: null
      }
    ];
  }
};
</script>

<style>
ul {
  text-align: left;
}
li {
  margin: 30px;
}
</style>