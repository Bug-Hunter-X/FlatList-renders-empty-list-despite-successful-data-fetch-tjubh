# React Native FlatList Empty List Bug

This repository demonstrates a common bug in React Native's FlatList component where the list remains empty even after successfully fetching data. The problem arises from an improperly configured `keyExtractor` function.

## Bug Description

The `DataList.js` file contains a component that fetches data from an API. Despite successful data retrieval, the FlatList remains empty.  The `keyExtractor` uses the index, which while seemingly simple, can cause problems under certain circumstances.

## Solution

The `DataListSolution.js` file presents a corrected version.  The solution uses a unique identifier from the fetched data as the key. This ensures that React Native can efficiently update the list when the data changes, preventing the empty list rendering issue.

## How to Reproduce

1. Clone this repository.
2. Navigate to the directory.
3. Run `npx react-native run-android` (or iOS equivalent).
4. Observe the empty list rendered by `DataList.js`.
5. Compare with the correctly functioning `DataListSolution.js`.

## Contributing

Contributions are welcome!