## 计算属性： 一个变量的值依赖于其他变量
### 场景： 订单的总价 = 数量*单价

```
   computed() {
     total() {
       return this.count * this.price
     }
   }

  ```
  ## 监听器 : 某个变量改变后触发某些动作
  ### 场景： 购物数量的加减限制
 ```
    watch:{
      activeIndex() {
        this.getList()
      }
    },
    count(){
      if(this.count<1) this.count = 1
    }

  ```

  ### creatd中请求ajax mounted中操作dom