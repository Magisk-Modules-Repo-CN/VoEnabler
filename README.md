## VoEnabler - 启用高清音视频通话
  
该模块通过修改`build.prop`的一些设置项来启用 VoLTE / VoWifi。  

**注意：** 如果你的运营商不支持 VoLTE/VoWiFi，那么就算你安装了本模块也不会有任何作用。
 [VoEnabler的XDA发布页](https://forum.xda-developers.com/apps/magisk/module-v4-volte-enabler-t3649613)

## 这个模块究竟做了啥事呢?

persist.dbg.ims_volte_enable=1 
<br>persist.dbg.volte_avail_ovr=1 
<br>persist.dbg.vt_avail_ovr=1
<br>persist.dbg.wfc_avail_ovr=1
<br>persist.radio.rat_on=combine
<br>persist.radio.data_ltd_sys_ind=1
<br>persist.radio.data_con_rprt=1
<br>persist.radio.calls.on.ims=1

也就是将以上这些加入Build


## 更新日志
2018-04-09 (v1.2): 更新Magisk模板至15+
<br>2017-08-02 (v1.1): 由于"persist.data.iwlan.enable=true"会导致经常性的断开Wifi以及数据网络的连接，所以移除了这条代码。
<br>2017-08-01 (v1): 从原本的使用Service.sh来执行脚本，改为直接写入build.prop
<br>2017-07-31 (Beta): 初次发布。
