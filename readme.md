#缩放地图无法改变自定义图层大小

##把自定义图层 看做一个图片 放在地图上

'''
//经纬度坐标转换为容器像素坐标
    AMap.event.addDomListener($('lng2x'),'click', function () {
        var px = lngX.value,py = latY.value;
        if (px && py) {
            var pixel = map.lnglatTocontainer([px, py]);
            pixelX.value = pixel.getX();
            pixelY.value = pixel.getY();
        }
    });

//drawImage 在画布上定位图像，并规定图像的宽度和高度：
    context.drawImage(img,x,y,width,height);

//
context.arc(x,y,r,sAngle,eAngle,counterclockwise);
'''