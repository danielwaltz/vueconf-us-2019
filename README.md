# Day 1 Workshop (Ridiculously Reusable Components)

- Components are nice (it is known)
- Slots are nice (it is known)
- Wrap vendor components for easier refactors
- Use `v-bind` for dynamically passing props
- Dollar sign not used in functional components
- Maybe use render function to pass down layout slots
- Look into [Codepilot repo](https://github.com/CodePilotai/codepilot) for inspiration
- Look into provide/inject
- Check out [Tailwind](https://github.com/tailwindcss/tailwindcss)

# Day 2

## State of the Vuenion

- Growing _fast_ (10% MoM) [State of Vue.js](https://www.monterail.com/state-of-vuejs-report)
- Use vue reactivity outside of component scope (advanced reactivity api)
- Mixins and HoCs are out - hook lyfe

## Intro to Nuxt

- Basically an opinionated Vue app starter
- Lots of performance configured for you out of the box
- Nuxt could be good option for marketing sites

## Vue.js In Practice

- Common theme - Vue is very incrementally adoptable
- Almost everyone has to maintain a legacy app (primarily Angular.js)
- Create a company specific vue cli plugin for shared functionality
- Code owners tool

## Vuex Explained Visually

- Use `mapState` and `mapGetters`

## Lightning Talks

### Progressive Validation

- Look into ValidityState api

### GraphQL Subscriptions

- Look into [Hasura](https://hasura.io/)

## Zen and the Art of Vue

- Forked templates with NativeScript looks like a great experience
- Vue cli plugin for NativeScript

## Demystifying: The Dark Art of SFC Compilation

- Custom template blocks are convenient
- Good use case is translations

## Phenomenal Design Patterns in Vue

- Dive into Design Patterns (book)

## The Future of Web Animation

- Make the web fun - anything can happen
- Pay attention to cognitive load
- Native 3D (AR/VR) is coming to browsers
- The web it stuck in blocks, design has become redundant

# Day 3

## Vue 3: What I'm Most Excited About

- Will be more simple and more explicit
- `Vue.set` for updating array items in Vue 2
- Vue 3 with proxies means you don't have to worry about it
- Multiple root node support!
- Emit `update` event instead of `input` for transparent wrappers in Vue 2
- In Vue 3, all you need is `v-bind="$attrs"` for v-model/listeners
- Vue 3 will no longer have attr inheritance (breaking change?)
- `v-on` will compile to attrs
- Vue 3 gets simpler render functions - closer to JSX
- Cool new Vue 3 features won't support IE
- Will be a Vue 3 migration tool that will offer to migrate code for you

## 9 Performance Secrets Revealed

- Use local variable based on computed prop value when using computed props together
- Prefer `v-show` over `v-if` when rendering is a concern
- Improve repeat route load by using special `<keep-alive>` component
- Use attrs to customize `<keep-alive>` for memory optimization
- Use defer to optimistically render parts of a route
- Use a queue to commit large payloads in chunks to a store like `vuex`
- You can opt out of reactivity for performance gains
- Use `<recycle-scroller>` lib for rendering large data sets
