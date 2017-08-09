# AndroidHelper

关于手机分辨率的dp问题：
  1. 布局设计以dp为基本单位
  2. dp的范围应该以初代android设备的160dpi设备，即1dp=1px为准
  3. 因此dp大致范围取决于density和dp的乘积即实际所占像素值，并受限于设备的分辨率（px*px）

关于不同设备相关的两个概念：
1. 如果是与布局layout相关的，根据手机尺寸予以区分：
  下面是上述4种泛化的屏幕尺寸对应的最小屏幕长宽尺寸。
  1. xlarge：960dp x 720dp
  2. large：640dp x 480dp
  3. normal：470dp x 320dp
  4. small：426dp x 320dp
  或者用最小宽度来区分：
  1. 320dp：典型的手机屏幕（如240x320 ldpi , 320x480 mdpi, 480x800 hdpi等）。
  2. 480dp：手机和平版电脑都可能使用的尺寸 (如480x800 mdpi)。
  3. 600dp：用于7英寸的平板电脑 （如Nexus 7的1280 x 800 ，介于mdpi 和hdpi之间）。
  4. 720dp:：用于10英寸的平板电脑 (如Nexus 10的2560×1600 ， 介于hdpi和xhdpi之间)。
2. 如果是与图像相关的，根据dpi予以区分：
  ldpi（低密度） 120dpi 
  mdpi（中密度） 160dpi 
  hdpi（高密度） 240dpi  
  xhdpi（扩展高密度） 320dpi
