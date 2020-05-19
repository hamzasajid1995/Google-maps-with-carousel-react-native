## Google maps with carousel - React native

React native project for google maps with carousel linked together

## Getting Started

To get started: 
```
yarn add
expo start
```

## Built With

* [React native maps](https://github.com/react-native-community/react-native-maps)
* [React native snap carousel](https://github.com/archriss/react-native-snap-carousel)

## Issues and solutions
- Sometimes carousel is not shown and setting the following prop resolves this
  ```
  removeClippedSubviews={false}
  ```
 // https://github.com/archriss/react-native-snap-carousel/issues/238, see description of method triggerRenderingHack() on githubb docs. setting false addreses issue where carosuel is not visible on first render.

- Use this prop to use Google maps on ios instead of apple maps for better performance:
  ```
  provider={MapView.PROVIDER_GOOGLE}
  ```
  
- Use flatlist instead of scrollview in carousel for lazy loading
  ```
  useScrollView={false}
  ```



## Demo
<img src="https://github.com/hamzasajid1995/google-maps-with-carousel-react-native/blob/master/demo/demo.gif?raw=true"  />

## Live working app use case

(Source Code for this project is private)

<img src="https://github.com/hamzasajid1995/google-maps-with-carousel-react-native/blob/master/demo/liveappdemo.gif?raw=true"  />
