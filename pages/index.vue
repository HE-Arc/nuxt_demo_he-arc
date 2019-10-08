<template>
  <div>
    <Navbar title="My Site"/>
    <Section title="What's your name?">
    <ReactivityTest/>
    </Section>
    <Section title="News">
      <News class="news" v-for="(el, idx) in news" :key="idx" :news="el"/>
    </Section>
  </div>
</template>

<script>
import Logo from '~/components/Logo.vue'
import Navbar from '../components/Navbar'
import Section from '../components/Section'
import News from '../components/News'
import ReactivityTest from '../components/ReactivityTest'


export default {
  layout: 'default',
  components: { ReactivityTest, News, Section, Navbar, Logo },
  data: () => ({
    news: [
      { title: "News", body: "Lorem ipsum dolor sit amet, consectetur adipisicing elit. Adipisci dolore expedita nemo odio quia quisquam sint. Aspernatur at, culpa delectus dignissimos ea, exercitationem odio optio perferendis quos sequi ut voluptatibus." },
      { title: "News", body: "Lorem ipsum dolor sit amet, consectetur adipisicing elit. Adipisci dolore expedita nemo odio quia quisquam sint. Aspernatur at, culpa delectus dignissimos ea, exercitationem odio optio perferendis quos sequi ut voluptatibus." },
      { title: "News", body: "Lorem ipsum dolor sit amet, consectetur adipisicing elit. Adipisci dolore expedita nemo odio quia quisquam sint. Aspernatur at, culpa delectus dignissimos ea, exercitationem odio optio perferendis quos sequi ut voluptatibus." },
      { title: "News", body: "Lorem ipsum dolor sit amet, consectetur adipisicing elit. Adipisci dolore expedita nemo odio quia quisquam sint. Aspernatur at, culpa delectus dignissimos ea, exercitationem odio optio perferendis quos sequi ut voluptatibus." },
      { title: "News", body: "Lorem ipsum dolor sit amet, consectetur adipisicing elit. Adipisci dolore expedita nemo odio quia quisquam sint. Aspernatur at, culpa delectus dignissimos ea, exercitationem odio optio perferendis quos sequi ut voluptatibus." },
      { title: "News", body: "Lorem ipsum dolor sit amet, consectetur adipisicing elit. Adipisci dolore expedita nemo odio quia quisquam sint. Aspernatur at, culpa delectus dignissimos ea, exercitationem odio optio perferendis quos sequi ut voluptatibus." },
    ]
  })

}
</script>

<style>

</style>
