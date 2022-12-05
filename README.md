# daming-nextjs-bazel-app

This is a [Next.js](https://nextjs.org/) project bootstrapped with [`create-next-app`](https://github.com/vercel/next.js/tree/canary/packages/create-next-app) and support [Bazel](https://bazelbuild.github.io/rules_nodejs/).

## Get started

use yarn

```bash
yarn build (next build)
yarn start (next start)
yarn dev (next dev)
```

use bazel

```bash
yarn bazel:build (ibazel run //:build)
yarn bazel:start (ibazel run //:start)
yarn bazel:dev (ibazel run //:dev)
```

## Questions

fail to use bazel run `next start` command

## Reference

1. [Bazel + next.js example](https://github.com/aspect-build/bazel-examples/tree/main/next.js)
2. [feat(examples) demonstrate building nextjs app](https://github.com/bazelbuild/rules_nodejs/pull/3297)
3. [bazel-next-typescript-monorepo](https://github.com/anthanh/bazel-next-typescript-monorepo)
4. [nextjs-bazel](https://github.com/flolu/nextjs-bazel)
