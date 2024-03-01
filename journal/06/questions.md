# Single Page Applications with Vue
01. What is the entrypoint of an application?

  > it's where we spin up or run an application from i.e. index.html or app.vue

02. What is the difference between a vue `component` and `page`?

  > a component is a small part of the app that can be outsourced where a page will contain all the content or refrences to the content displayed to the user on a single page.

03. What is ***Component-Based Architecture***?

  > Component-Based Architecture is where we out source the code to reusable components.

04. What are the three tags that make up a Vue component?

  > The three tags that make up view are 
  > 🔵 template - which enables html
  > 🔴 script - which enables javascript 
  > 🟢 style - which enable css styling on default

05. What are ***lifecycle hooks***? What are lifecycle hooks used for?

  > Lifecycle hooks track information behind the scenes and allows us to draw, create, update or destroy components. 
   
06. Which component in Vue does the vue-router use to mount pages onto?

  > App.vue

07. What is the difference between the `AppState` and the state object within a component?

  > the AppState contains reactive data and variables across the entire app, where as the state contains data specific to that component 

08. What is the responsibility of `Services` in our Vue projects?

  > to change information in the state or the AppState

09. What are ***props*** and how are they used? Provide an example

  > Props are similar to arguments and parameters in the fact that they are passed down to components in a similar manner. they are read only, and cannot be passed (back) up because we are using vue. you instead 'prop' them up to be used by the parent component
  >
  ```html
  <!-- Parent  -->
  <template>
    <!-- each property is a prop -->
    <Banner
      :name="Seth"
      :description="is cool"
      :age="20"
    /> 
  </template>

  <script>
    export default {
      name: 'Banner',
      props: {
        name: {
          type: String,
          required: true,
        }
        description: {
          type: String,
        }
        age: {
          type: Number,
        }
        },
    }
  </script>

  <!-- child "Banner"-->
  <template>
    <div class="banner card">
  <!-- I don't really grasp how it's passed down, but this is what it looks like after being passed down -->
      <h2 class="banner_name"></h2>
      <p>
      <span class="banner_description"></span>
      <span class="banner_age"></span>
      </p>
    </div>
  </template>
  ```

10. What is the Vue method used to create watchable objects such as `state` or `AppState`?

  >
  ```js 
  export default {
    // this part is the vue method used to create watchable objects that can be accessed
    setup() {
      return state
    }
  }
  ```