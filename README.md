# Atom Redux Duck Snippets
Atom Snippets for [Redux Duck](https://github.com/sergiodxa/redux-duck). This snippets uses Babel(ES2015, ES2016) syntax.

## Support Language

- Babel (ES2015, ES2016)

## Usage

- Import Redux Duck (`duck-ipt`)
```js
import { createDuck } from 'redux-duck';
```
- Create Redux Duck (`duck-crt`)
```js
const duck = createDuck('$1', '$2')$3
```
- Define Duck Action Type (`duck-tp`)
```js
const $1 = duck.defineType('$1');$2
```
- Create Action Creator (`duck-act`)
```js
/**
 * Create $1 action object
 * @params  {Object} payload Action data
 * @returns {Object}         Action object
 */
export const $2 = duck.createAction($1);$3
```
- Create Reducer (`duck-rdc`)
```js
/**
 * $1
 * @param  {Object} state  Actual state object
 * @param  {Object} action Changes to apply
 * @return {Object}        New state object
 */
export default duck.createReducer({
  ${3:duck-case}
}, $2);
```
- Create Reducer action case (`duck-case`)
```js
[$1]: (state, { payload = {} }) => {
  ${2:return state;}
},$3
```

## LICENSE

[MIT](LICENSE)
