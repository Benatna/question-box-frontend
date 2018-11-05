<template>
  <section>
    <div class="container about-title">
      <h1 v-html="$t('about.title')"></h1>
    </div>
    <div>
      <img src="../assets/about_project.jpg" class="fullwidth-image" alt="Picture of Young People">
    </div>
    <div class="text-over-image">
      <i18n path="about.description" tag="p" class="about-description">
        <em>{{$t('app.app_name')}}</em>
        <router-link :to="{ name: 'ambassadors' }">{{$t('about.young_people')}}</router-link>
      </i18n>
    </div>
  </section>
</template>

<script>

export default {
  name: 'About'
}
</script>

<style>

.about-title {
  margin-bottom: 30px;
}

.about-description {
  margin: 0;
  font-size: 20px;
  line-height: 30px;
}

.about-team {
  margin: 0 auto 50px auto;
}

.about-team p {
  margin-top: 0;

}

</style>
