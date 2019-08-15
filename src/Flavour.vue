<!--
  ~ Copyright (c) 2018, 2019 Oracle and/or its affiliates. All rights reserved.
-->
<template>
<v-container v-bind:id="id" fluid light class="slide_flavour">
    <v-layout row wrap>
        <v-flex md2 class="hidden-sm-and-down" />
        <v-flex md4 xs12 class="panel">
            <v-container fluid light>
                <v-flex md11 xs12>
                    <div class="logo-graphics helidon-se-logo"></div>
                    <div class="section">
                        <div>
                            <ul>
                                <li>Reactive microframework</li>
                                <li>Tiny footprint</li>
                                <li>Functional style APIs</li>
                                <li>No magic involved</li>
                                <li>Supports GraalVM</li>
                            </ul>
                        </div>
                    </div>
                    <div class="button-panel">
                        <v-btn light
                               large
                               href="./docs/latest/#/guides/01_overview"
                               target="_blank"
                               rel="noopener">Getting Started</v-btn>
                    </div>
                </v-flex>
                <v-flex md1 class="hidden-sm-and-down" />
            </v-container>
        </v-flex>
        <v-flex md4 xs12 class="panel">
            <v-container fluid light>
                <v-flex md1 class="hidden-sm-and-down" />
                <v-flex md11 xs12>
                    <div class="logo-graphics helidon-mp-logo"></div>
                    <div class="section">
                        <div>
                            <ul>
                                <li>MicroProfile Implementation</li>
                                <li>Small Footprint</li>
                                <li>Declarative style APIs</li>
                                <li>Dependency Injection</li>
                                <li>CDI, JAX-RS, JSON-P/B</li>
                            </ul>
                        </div>
                    </div>
                    <div class="button-panel">
                        <v-btn light
                               large
                               href="./docs/latest/#/guides/01_overview"
                               target="_blank"
                               rel="noopener">Getting Started</v-btn>
                    </div>
                </v-flex>
            </v-container>
        </v-flex>
        <v-flex md2 class="hidden-sm-and-down" />
    </v-layout>
</v-container>
</template>
<script>
export default {
  props: {
    id: {
      type: String,
      required: true
    }
  }
}
</script>
<style lang="sass">
  .panel
    :margin-bottom: 50px
  .slide_flavour
    :background-color #41a8ff
    :padding-top 100px
    :padding-bottom 50px
    .section
      :margin-left auto
      :margin-right auto
      :min-height 200px
      :display table
      div
        :margin-left auto
        :margin-right auto
        :display table-cell
    .button-panel
      :text-align: center
      :margin-top: 30px
    p
      :color white
      :font-size 1.5em
    ul
      :margin-left 50px
    li
      :font-size 1.5em
      :color white
    .logo-graphics
      :margin-left auto
      :margin-right auto
      :background-position: 50% 50%
      :background-size: contain
      :height: 120px
      :max-width: 400px
    .helidon-se-logo
      :background-image url('../static/img/helidon_SE_white.png')
    .helidon-mp-logo
      :background-image url('../static/img/helidon_MP_white.png')
</style>
