```
    <div class="imageDom" ref="imageDom"此处是里面的内容</div>

    //JS部分
    import html2canvas from "html2canvas"
    data(){
        imgUrl:''
    },
    methods:{
        savePhoto(){
            html2canvas(this.$refs.imageDom,{
                backgroundColor:'#eee' //设置生成的图片背景色，默认是白色
            }).then(canvas => {
                //将生成的canvas转成base64编码图片
                this.imgUrl = canvas.toDataURL("images/png"); 
            });
        }
    }

```
###注意，如果生成图片的内容里面有背景图，背景图引入地址需要改成相对本地的，不然，生成的图片不会显示