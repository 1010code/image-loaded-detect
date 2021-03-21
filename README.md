# image-loaded-detect
load the image using Javascript, and then set that image as the backgroud.

```js
// 建立一張照片
var bgImg = new Image();
// 當圖片載入完成時執行onload function
bgImg.onload = function () {
    console.log('載入完成！');
    // 在body放入背景圖位置
    document.body.style.backgroundImage = 'url(' + bgImg.src + ')';
    // 停止loading動畫
    document.getElementById('load-wrapper').classList.add('d-none');
};
// 指定圖片來源位置
bgImg.src = 'https://effigis.com/wp-content/uploads/2015/02/DigitalGlobe_WorldView1_50cm_8bit_BW_DRA_Bangkok_Thailand_2009JAN06_8bits_sub_r_1.jpg';
```

## Copyright of the Image
- Image Source: [Effigis](https://effigis.com/en/solutions/satellite-images/satellite-image-samples/)
- Bangkok, Thailand
- Sensor: WorldView-1
- Resolution: 50 cm
- Image size: 15 MB