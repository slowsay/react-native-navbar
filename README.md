# react-native-navbars

> 顶部导航组件,分为左(返回),中(标题),右(分享),三部分填充内容.一般与navigator配合使用
> 主要是继承概念,代码规整，方便代码多次重用,对于性能暂无更好的优化方案

[![NPM](https://nodei.co/npm/react-native-navbars.png)](https://nodei.co/npm/react-native-navbars/)

## Install
#### Ios
npm install --save react-native-navbars
#### android
暂无

## Example

```
import Headnavbar from 'react-native-navbars';

export default class extends Component {
    render(){
        reutrn(
         <Headnavbar title='新闻' tintColor="#f0f0f0" onhandle={()=>console.log('ok')} navigator={navigator}/>
         )
     }
}
```

## Api props

### title
顶部导航栏标题

### tintColor
背景颜色

### onhandle
右侧按钮,触发click事件

### navigator
导航props组件绑定

### leftbutton
左侧菜单属性,
- leftbutton.title 标题
- leftbutton.tintColor 标题颜色

```
<Headnavbar title='新闻' leftbutton={{title:'like',tintColor:'#ff0'}} tintColor="#f0f0f0" onhandle={()=>console.log('ok')} navigator={navigator}/>
```

### rightbutton
右侧菜单属性
- rightbutton.title 标题
- rightbutton.tintColor 标题颜色
```
以此类推
```

## Version

- v0.0.1 update
