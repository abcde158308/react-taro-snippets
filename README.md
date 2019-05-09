
# react-taro-snippets

[![Version](https://vsmarketplacebadge.apphb.com/version/liulei.react-taro-snippets.svg)](https://marketplace.visualstudio.com/items?itemName=liulei.react-taro-snippets)
[![Install](https://vsmarketplacebadge.apphb.com/installs-short/liulei.react-taro-snippets.svg)](https://marketplace.visualstudio.com/items?itemName=liulei.react-taro-snippets)


用JS的格式,但是智能提示响应范围包括如下

- `typescript`
- `javascript`
- `javascriptreact`
- `typescriptreact`

部分位置设置了占位符,可以初始化的时候修改及`tab`切换


-----

# 效果

![演示Demo](images/show.gif)


---

# 代码片段

- `reactts`

```javascript
import React, { Component } from 'react'
import { connect } from 'react-redux'
//import * as actions from './storeModel/actionCreater'

interface Props {
}
interface State {
}
class  Index extends Component <Props, State> {
    constructor(props:Props){
       super(props);
        this.state = {
        }
    }
    render() {

        return (
            <div className='component-Index'>

            </div>
        )
    }
}

const mapState = (state) => ({

})

const mapDispatch = (dispatch) => ({

})

export default connect(mapState, mapDispatch)(Index);
```

- `tarocc`

```javascript
import Taro , { Component } from '@tarojs/taro';
import { View, Text , Button} from '@tarojs/components';

export default class Index extends Component {

   config = {
       navigationBarTitleText: ''
  }

  state={}

  componentWillMount () {}
  componentDidMount () {}
  componentWillReceiveProps (nextProps,nextContext) {}
  componentWillUnmount () {}
  componentDidShow () {}
  componentDidHide () {}
  componentDidCatchError () {}
  componentDidNotFound () {}
  render() {
    return (
      <View>

      </View>
    );
  }
}
export default Index;

```
- `tarots`

```javascript 
import { ComponentClass } from 'react'
import Taro, { Component } from '@tarojs/taro'
import { View ,Text } from '@tarojs/components'
import './Figure.less'

type PageStateProps = {}

type PageDispatchProps = {}

type PageOwnProps = {}

type PageState = {
    name: string
}

type IProps = PageStateProps & PageDispatchProps & PageOwnProps

interface Figure {
    props: IProps;
    state: PageState
}

class Figure extends Component {
   constructor(props){
       super(props)
       this.state = {
          name: '小红'
       }

    }
componentWillReceiveProps (nextProps) {}

componentWillUnmount () { }

componentDidShow () { }

componentDidHide () { }

render () {
    return (
        <View className='Figure'>
            <Text>hello world</Text>
        </View>
    )
}

}
export default Figure as ComponentClass<PageOwnProps, PageState>
```

- `taropc`


```javascript

import Taro , { PureComponent } from '@tarojs/taro';
import { View, Text , Button} from '@tarojs/components';

class Index extends PureComponent {

   config = {
       navigationBarTitleText: ''
  }

  state={}

  componentWillMount () {}
  componentDidMount () {}
  componentWillReceiveProps (nextProps,nextContext) {}
  componentWillUnmount () {}
  componentDidShow () {}
  componentDidHide () {}
  componentDidCatchError () {}
  componentDidNotFound () {}
  render() {
    return (
      <View>

      </View>
    );
  }
}
export default Index;

```

- `taroaf`


```json
config = {
  pages: [
    'pages/index/index'
     ],
  window: {
    backgroundTextStyle: 'light',
    navigationBarBackgroundColor: '#fff',
    navigationBarTitleText: 'WeChat',
    navigationBarTextStyle: 'black'
    }
}

```

- `taroimd`

```javascript
import {} from '@tarojs/mobx'
```


- `taroird`

```javascript
import {} from '@tarojs/redux'
```

- `taroimm`

```javascript
import {} from '$tarojs/'
```


- `taroir`


```javascript
import { connect } from '@tarojs/redux'
```


- `taroim`


```javascript
import {inject, observer} from '@tarojs/mobx'
```

- `imo`

```javascript
import { action, observable, computed, toJS } from 'mobx'
```


---

# 其他


有问题的小伙伴可以提交`PR`
