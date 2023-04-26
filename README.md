# vue-emits-issue

- the repo is created by `pnpm create vite` withe default Typescript

## steps to reproduce

- change the return value of the event `submit()` in `defineEmits` in `Comp.vue`
- click the `Comp Button` and see the warn in browser console

## What is expected?

The warn should display correctly after the return value of the event without refresh.

## What is actually happening?

The warn always displays when the default return is false. It will not disappear after the return value has been changed to true without refresh.

Also, the `defineProps` has the same issue.

## related docs

<https://cn.vuejs.org/guide/components/events.html#declaring-emitted-events>