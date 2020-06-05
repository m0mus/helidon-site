<!--
  ~ Copyright (c) 2020 Oracle and/or its affiliates. All rights reserved.
-->
<template>
  <v-container grid-list-md text-xs-center class="features2_slide">
    <v-layout row wrap class="section">
      <v-flex xs12>
        <h2>Helidon 2.0 Highlights</h2>
        <div class="graalvm-logo"></div>
        <p class="one_sentence">GraalVM native-image support in both Helidon SE and Helidon MP</p>
      </v-flex>
    </v-layout>
    <v-layout row wrap class="section">
      <v-flex xs12>
        <h2>Helidon 2.0 Highlights</h2>
        <h3>Helidon Command Link Utility</h3>
        <div class="cli-img"></div>
        <p>Read more</p>
      </v-flex>
    </v-layout>
    <v-layout row wrap class="section">
      <v-flex xs12>
        <h2>Helidon 2.0 Highlights</h2>
        <h3>Helidon SE DBClient</h3>
        <ul>
            <li>Reactive non-blocking database client</li>
            <li>Supports existing blocking JDBC drivers</li>
            <li>Relational and non-relational databases</li>
            <li>Metrics, tracing, health checks</li>
            <li>Portability</li>
            <li>Extensibility</li>
        </ul>
      </v-flex>
    </v-layout>
  </v-container>
</template>
<script>
  export default {
    props: {
      backgroundColor: {
        type: String,
        default: 'transparent'
      },
      color: {
        type: String,
        default: 'white'
      },
      paddingTop: {
        type: Number,
        default: 0
      },
      paddingBottom: {
        type: Number,
        default: 0
      }
    }
  }
</script>
<style lang="sass">
  .features2_slide
    .section
      :padding-top 10vh
      :padding-bottom 10vh
      :text-align center
    h2
      :color #3ea5fd
      :text-align center
      :font-weight 400
      :font-size 3em
      :margin-bottom 80px
    h3
      :color #595959
      :font-weight 400
      :font-size 2em
    .one_sentence
      :color #797979
      :margin-top: 50px
      :margin-bottom 80px
      :font-size 5em
    .graalvm-logo
      :height: 200px
      :background-position: 50% 50%
      :background-image url('../static/img/graalvm_logo.svg')
    .cli-img
      :height: 530px
      :background-position: 50% 50%
      :background-image url('../static/img/cli.png')
</style>
