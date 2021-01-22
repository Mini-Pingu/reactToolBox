# React ToolBox

根據公司購買的 [**Shards Dashboard Pro React**](https://designrevision.com/downloads/shards-dashboard-pro-react/) 套件，將其中每一個 View 都吃透它。具體做法就是對 Shards 使用到實用性爆表的庫都玩得很6。坦白說，這個套件只是一個懶人包，因爲要用 React 做出很好看的效果，還是要看自身的實力，`Shards` 只是加速了一些過程進度，譬如 `Styles`，`CSS`,  Flux 等。只能說這是一個高級付費版的 React 腳手架。可以學習的東西還是有很多的。MVC 結構就是其中之一。

因爲知識產權的問題（或者我猜我會因爲直接可能 push 付費的源碼而惹上官司），所以我只會在 toolbox 中從 0 自己寫一次就好了。

## 目標任務列表

任務的順序就是：

- 先按照 routes.js export 的 router 一個 view 一個 view 地掃，把每個 view 中用到的 component 都弄明白。
- 之後在看其他的。（暫時還沒有計劃，先把 router 的看完，基本上就看了個 七成了）

### /analytics

#### 庫

`<Sessions />` 最重要的是 `react-chartjs-2` 的用法

1. [`chart.js`](https://www.chartjs.org/)
2. [`react-chartjs-2 `](https://openbase.com/js/react-chartjs-2) =>  [example](https://reactchartjs.github.io/react-chartjs-2/#/) (只要在需要的時候，再從這裏 copy & paste 就好了)

` <CountryReports />` 的中心思想就是把地圖展現出來，然後賦值給每個地區，可是用的是 `createRef` 直接控制 DOM，看看有沒有其他替代（容易）的方法

1. 可以試試這個 [`google-map-react`](https://github.com/google-map-react/google-map-react#examples)
2. 善於利用 [Google Maps Platform](https://developers.google.com/maps/)
3. 國內還是使用 [`react-amap`](https://github.com/ElemeFE/react-amap) 高德地圖比較好



- 要知道 `React.createRef()` 是做什麼的
- color 是需要獨立放在 另外一個 config / util 的 file 裏最好

## 其他

1. `react-router-dom` 中 Route 的 `route.layout` 和 `route.component`
2. [`react-ga`](https://github.com/react-ga/react-ga)

