# Managing the Fullstack Application

1. Describe the two ways to bind Data in Vue?

  > v-bind and shorthand
  ```vue
  <!-- v-bind longhand -->
   <div v-bind:attribute="object.property"> </div>
   <!-- v-bind shorthand -->
   <div :attribute="object.property"></div>
  ```

2. The `SPA` acronym stands for what?

  > single page aplication

3. What are some of the advantages/uses of a `SPA` over a traditional one?

  > designed to be more reactive

4. What does the `onMounted` method in Vue do?

  > runs on page mount

5. What is the `v-model` attribute in Vue for, and when might you use it?

  > used for two way data binding, allows someone to fill out an input where the input updates even before submitting. if you want a reactive input and variable you would use a v-model

6. What is the package.json file used for?

  > sets up parameters for which versions of each technology the application wil be using to work correctly

7. Which Vue attributes(directives) could you use to conditionally render elements on a page?

  > v-if, v-bind, v-model, and v-for all render objects onto the page based on a condition.

8. What is the purpose of the `key` attribute when using `v-for` on an element?

  > to Identify the part in an array on instance without refrencing the instance number

9. What is the `<slot>` element and what is it used for?

  > an element that users can use to fill in their own markup
