# React VirtualSky

Its react version of [VirtualSky](https://github.com/slowe/VirtualSky).


## Usage

```jsx
export default class App extends React.Component {

  const azOff = 0;
  const height = 500;
  const width = 500;
  const latitude = 51.746449;
  const longitude = 19.620693;
  const time = new Date();
  const config = projectionsConfig(args.width, args.height-50, args.latitude, args.longitude, args.time)

  render() {
    return <VirtualSky id="startmap" config={config} azOff={args.azOff}/>
  }
}
```

## Development

```
cd react-trello/
yarn install
yarn run storybook
```

### Scripts

1.  `yarn run lint` : Lint all js files
2.  `yarn run lintfix` : fix linting errors of all js files
3.  `yarn run semantic-release` : make a release. Leave it for CI to do.
4.  `yarn run storybook`: Start developing by using storybook
5.  `yarn run test` : Run tests. tests file should be written as `*.test.js` and using ES2015
6.  `yarn run test:watch` : Watch tests while writing
7.  `yarn run test:cover` : Show coverage report of your tests
8.  `yarn run test:report` : Report test coverage to codecov.io. Leave this for CI
9.  `yarn run build`: transpile all ES6 component files into ES5(commonjs) and put it in `dist` directory
10. `yarn run docs`: create static build of storybook in `docs` directory that can be used for github pages

Learn how to write stories [here](https://storybook.js.org/basics/writing-stories/)
