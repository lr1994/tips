```
    <canvas id="canvas" class="shareIcon"/>
    import QRCode from 'qrcode'

    makeEwm(){
        let canvas = document.getElementById('canvas')
        let src = document.location.href;
        QRCode.toCanvas(canvas,src,{
            width:70,
            height:70
        },(err)=>{
            if(err) console.log(err)
        })
    }
```