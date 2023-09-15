# turborepo + react native sample

[Buildless][1], [Pkgst][8], [Turbo][2], and [React Native][3] with [sccache][4].


## Details about this sample

Together, these tools provide a unified cross-platform development environment, enabled with blazing-fast remote build caching. Turbo handles build caching for the web portion of the app. `sccache` kicks in for Swift builds.


### Additional resources

- [Buildless docs: Turborepo setup][7]
- [Swift docs: Using `sccache`][5]
- [Turbo docs: Remote caching][9]


## Using this example

> **Before you start:** Obtain an API key for [Buildless][1], set it at `BUILDLESS_APIKEY` in your environment

1) Clone the sample, install dependencies with `pnpm i`
2) Run a build with `pnpm run build`; observe that Turbo uses Buildless
3) Set up [`sccache`][4], and [link it to your Swift toolchain][5]
4) Enjoy lightning-fast builds on all platforms


### Building and running each app

> To run the web app:
```
pnpm run dev
```

> To run the iOS app:
```
pnpm run ios
```

> To run the Android app:
```
pnpm run android
```


## Docs from the original template

This template is a fork of [a similar Vercel-provided template][6]. The original README docs from that template are enclosed below.

### What's inside?

This Turborepo includes the following packages/apps:

### Apps and Packages

- `native`: a [react-native](https://reactnative.dev/) app built with [expo](https://docs.expo.dev/)
- `web`: a [Next.js](https://nextjs.org/) app built with [react-native-web](https://necolas.github.io/react-native-web/)
- `ui`: a stub [react-native](https://reactnative.dev/) component library shared by both `web` and `native` applications
- `tsconfig`: `tsconfig.json`s used throughout the monorepo

Each package/app is 100% [TypeScript](https://www.typescriptlang.org/).

### Utilities

This Turborepo has some additional tools already setup for you:

- [Expo](https://docs.expo.dev/) for native development
- [TypeScript](https://www.typescriptlang.org/) for static type checking
- [Prettier](https://prettier.io) for code formatting


[1]: https://less.build
[2]: https://turbo.build
[3]: https://reactnative.dev
[4]: https://github.com/mozilla/sccache
[5]: https://github.com/apple/swift/blob/main/docs/DevelopmentTips.md#use-sccache-to-cache-build-artifacts
[6]: https://vercel.com/templates/next.js/turborepo-react-native
[7]: https://docs.less.build/docs/turborepo
[8]: https://docs.less.build/docs/pkgst
[9]: https://turbo.build/repo/docs/core-concepts/remote-caching
