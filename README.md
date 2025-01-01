# React Native FlatList Data Update Bug

This repository demonstrates a common bug encountered when working with `FlatList` in React Native. The issue arises when updating the data source, where the `FlatList` component fails to re-render properly, leading to inconsistencies in displayed data. This often happens with incremental updates or modifications that don't alter the data source's length.

## Bug Description
The provided `bug.js` file shows a `FlatList` component that doesn't consistently re-render when its data source is updated.  This results in stale data being displayed.

## Solution
The `bugSolution.js` file offers a solution that ensures proper re-rendering by using a unique key for each item and leveraging the `extraData` prop.