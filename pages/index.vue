<template>
  <b-container class="my-5">
    <b-row>
      <b-col cols>
          <h4>Featured Announcements</h4>
      </b-col>
    </b-row>
    <b-row>
      <b-col cols="5">
        <featured-announcements></featured-announcements>
        <b-row class="mt-4">
          <b-col cols>
            <h4>Pinned Announcements</h4>
          </b-col>
        </b-row>
        <pinned-announcements></pinned-announcements>
        <announcements class="mt-3"></announcements>
      </b-col>
      <b-col cols="7" class="pl-1">
        <b-row>
          <b-col cols="4" class="pr-1">
            <profile></profile>
          </b-col>
          <b-col cols="8">
            <story></story>
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
