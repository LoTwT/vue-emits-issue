# vue-emits-issue

- the repo is created by `pnpm create vite` withe default Typescript

## steps to reproduce

- change the return value of the event `submit()` in `defineEmits` in `Comp.vue`
- click the `Comp Button` and see the warn in browser console

## What is expected?

The warn should output correctly after the return value of the event changed without refresh.

## What is actually happening?

The warn always outputs after the return value changed from `false` to `true`. It will be correct after refreshing.

Also, the `defineProps` has the same issue.

## related docs

<https://cn.vuejs.org/guide/components/events.html#declaring-emitted-events>