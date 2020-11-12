# Yarn Workspaces with Lerna

Lerna is not obsolete now that this can be handled much easier with workspaces.

Lerna still comes in handy whenever you actually want to do something with your packages. Be it publishing them, running test or any other arbitrary scripts over them. You name it. Lerna actually ties in really well with yarn

## Installation

Globally install Yarn:

```bash
npm -g yarn lerna
```

Use the bootstrap we build here:

```bash
yarn bootstrap
```

## Usage

Run storybook by running:

```bash
yarn dev
```

## Testing

Run testing by running:

```bash
yarn unit
```

and

```bash
yarn coverage
```

## Publishing

Let’s release the first version of our packages. We can use npx lerna changed
to see which packages have changed. You can also use npx lerna diff to see
specifically what lines changed.

```bash
lerna diff
```

We can see it recognizes both the button and the input package. Now, let’s run
npx lerna version to simulate releasing them.

```bash
lerna version
```

If we wanted to release our packages to NPM, we would use npx lerna publish instead.

```bash
lerna publish
```

## Contributing

TBC

## License

[MIT](https://choosealicense.com/licenses/mit/)

Futher reading
https://leerob.io/blog/monorepo-lerna-yarn-workspaces
https://leerob.io/blog/ui-component-library-with-styled-components
https://yarnpkg.com/blog/2017/08/02/introducing-workspaces/
https://planflow.dev/blog/what-is-a-yarn-workspace
https://www.devbridge.com/articles/a-step-by-step-build-to-build-a-sharable-components-library/
https://docs.npmjs.com/creating-and-publishing-private-packages
https://www.julianburr.de/til/lerna-and-yarn-workspaces/
https://medium.com/ah-technology/a-guide-through-the-wild-wild-west-of-setting-up-a-mono-repo-with-typescript-lerna-and-yarn-ed6a1e5467a
