# @urql/vue

## 0.2.1

### Patch Changes

- Add a built-in `gql` tag function helper to `@urql/core`. This behaves similarly to `graphql-tag` but only warns about _locally_ duplicated fragment names rather than globally. It also primes `@urql/core`'s key cache with the parsed `DocumentNode`, by [@kitten](https://github.com/kitten) (See [#1187](https://github.com/FormidableLabs/urql/pull/1187))
- Updated dependencies (See [#1187](https://github.com/FormidableLabs/urql/pull/1187), [#1186](https://github.com/FormidableLabs/urql/pull/1186), and [#1186](https://github.com/FormidableLabs/urql/pull/1186))
  - @urql/core@1.16.0

## 0.2.0

### Minor Changes

- Export a Vue plugin function as the default export, by [@LinusBorg](https://github.com/LinusBorg) (See [#1152](https://github.com/FormidableLabs/urql/pull/1152))
- Refactor `useQuery` to resolve the lazy promise for Vue Suspense to the latest result that has been requested as per the input to `useQuery`, by [@kitten](https://github.com/kitten) (See [#1162](https://github.com/FormidableLabs/urql/pull/1162))

### Patch Changes

- ⚠️ Fix pausing feature of `useQuery` by turning `isPaused` into a ref again, by [@LinusBorg](https://github.com/LinusBorg) (See [#1155](https://github.com/FormidableLabs/urql/pull/1155))
- ⚠️ Fix implementation of Vue's Suspense feature by making the lazy `PromiseLike` on the returned state passive, by [@kitten](https://github.com/kitten) (See [#1159](https://github.com/FormidableLabs/urql/pull/1159))

## 0.1.0

Initial release
