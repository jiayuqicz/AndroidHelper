# AndroidHelper
关于手机分辨率的dp问题：
1. 布局设计以dp为基本单位
2. dp的范围应该以初代android设备的160dpi设备，即1dp=1px为准
3. 因此dp大致范围取决于density和dp的乘积即实际所占像素值，并受限于设备的分辨率（px*px）
