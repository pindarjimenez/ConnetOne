<template>
  <b-container class="my-5">
    <b-row>
      <b-col cols>
          <h4>Featured Announcements</h4>
      </b-col>
    </b-row>
    <b-row>
      <b-col cols md="5">
        <featured-announcements></featured-announcements>
        <b-row class="mt-4">
          <b-col cols>
            <h4>Pinned Announcements</h4>
          </b-col>
        </b-row>
        <pinned-announcements></pinned-announcements>
        <announcements class="mt-3"></announcements>
      </b-col>
      <b-col cols md="7" class="pl-md-1 mt-3 mt-md-0">
        <b-row>
          <b-col cols sm="4" class="pr-md-1">
            <profile></profile>
          </b-col>
          <b-col sm="8">
            <story class="mt-3 mt-sm-0"></story>
            <post class="mt-3"></post>
          </b-col>
        </b-row>
        <b-row>
          <b-col cols class="mt-3">
            <news-feed></news-feed>
          </b-col>
        </b-row>
      </b-col>
    </b-row>
  </b-container>
</template>

<script>
export default {}
</script>

<style>
  body {
    background-color: #f0f4ff;
  }
</style>
