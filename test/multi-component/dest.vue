<script>
import Vue from 'vue'
const PunComponent0 = Vue.extend({
  template: `<h3 class="pun-title">This is pun-loader test 1</h3>`,
  components: {}
})
const PunComponent1 = Vue.extend({
  template: `<section class="pun-section">      <h3 class="pun-title">This is pun-loader test</h3>      <p>Funds donated via Patreon go directly to support Evan You&apos;s full-time work on Vue.js.</p>      <button @click="echo">Click</button>    </section>`,
  methods: {
    echo() {
      console.log('Click event trigger')
    }
  },
  components: {}
})
const PunComponentTestOne = Vue.extend({
  template: `<h3 class="pun-title">This is pun-loader test 1</h3>`,
  components: {}
})
export default {
  methods: {
    echo() {
      console.log('Click event trigger')
    }
  },
  data: function() {
    return {
      PunCode: {
        '0': {
          template: '<h3 class="pun-title">This is pun-loader test 1</h3>',
          script: '',
          style: '.pun-title {\n      color: #333;\n    }'
        },
        '1': {
          template:
            '<section class="pun-section">\n      <h3 class="pun-title">This is pun-loader test</h3>\n      <p>Funds donated via Patreon go directly to support Evan You&apos;s full-time work on Vue.js.</p>\n      <button @click="echo">Click</button>\n    </section>',
          script:
            "export default {\n      methods: {\n        echo () {\n          console.log('Click event trigger')\n        }\n      }\n    }",
          style: {
            '0': '.pun-title {\n        color: #f00;\n      }',
            '1':
              '.pun-section {\n        background-color: #000;\n        color: #fff;\n      }'
          }
        },
        testOne: {
          template: '<h3 class="pun-title">This is pun-loader test 1</h3>',
          script: '',
          style: '.pun-title {\n      color: #333;\n    }'
        }
      }
    }
  },
  components: { PunComponent0, PunComponent1, PunComponentTestOne }
}
</script>              <style>
.pun-title {
  color: #333;
}
</style>                  <style scoped>
.pun-title {
  color: #f00;
}
</style>                  <style>
.pun-section {
  background-color: #000;
  color: #fff;
}
</style>
