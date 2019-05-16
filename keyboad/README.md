# tips
some useful tips
````
 <input placeholder="请输入手机号" v-model="phone" maxlength="11" pattern="[0-9]\*"  @blur="blurIpt" />
 methods:{
          blurIpt(){
            
            document.documentElement.scrollTop = 0;
            document.body.scrollTop = 0;
        },
}
````
