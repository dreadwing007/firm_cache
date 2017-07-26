# firm_cache
firmware cache from DJI Assistant.app 
as extracted from dji_system.bin files, and collected by end users. 
Accompanying .bin files can be located here: https://github.com/MAVProxyUser/dji_system.bin

<img src=https://media.giphy.com/media/wNR8ZhO4fObRu/giphy.gif>

### Individual .cfg.sig 
```
MD5 (V01.00.0300_Spark_dji_system/wm100a.cfg.sig) = 0cf4d32c2cad2818a3daf4fe8ef4b554
MD5 (V01.00.0330_I2_dji_system/01.00.0330.cfg.sig) = 994836302ec9679a5519144d927e0712
MD5 (V01.00.0400_Spark_dji_system/wm100a.cfg.sig) = 89acae2e291ebd0d4d57fbc4e9d4a0b0
MD5 (V01.01.0010_I2_dji_system/wm620.cfg.sig) = e3b656cb06682e0ee7e1636b0adcf569
MD5 (V01.02.0602_P4_dji_system/wm330.cfg.sig) = 00dbe5966e3d5d97860aa3ad2251b85a
MD5 (V01.03.0200_Mavic_dji_system/wm220.cfg.sig) = 9a0e3cc7b2cddc18db2c10cd18b5c07b
MD5 (V01.03.0200_RC_Mavic_dji_system/wm220_rc.cfg.sig) = 9a0e3cc7b2cddc18db2c10cd18b5c07b
MD5 (V01.03.0400_Mavic_dji_system/wm220.cfg.sig) = 545c830c4b073efe667c664d0e169988
MD5 (V01.03.0400_RC_Mavic_dji_system/wm220_rc.cfg.sig) = 545c830c4b073efe667c664d0e169988
MD5 (V01.03.0500_Mavic_dji_system/01.03.0500.cfg.sig) = ad291d8a3bb74b8c3cb09d2d7fb83277
MD5 (V01.03.0509_P4P_dji_system/wm331_ac_fw_v01-03-0509.cfg.sig) = ad7ebd830435dfd1c2cb09c66bc9b019
MD5 (V01.03.0550_Mavic_dji_system/wm220.cfg.sig) = 1e6263009dee150d62b53c292bcf8ea4
MD5 (V01.03.0550_RC_Mavic_dji_system/wm220_rc.cfg.sig) = 1e6263009dee150d62b53c292bcf8ea4
MD5 (V01.03.0600_Mavic_dji_system/wm220.cfg.sig) = 8289a6d410b542f6c41a08bcfe8473aa
MD5 (V01.03.0600_RC_Mavic_dji_system/wm220_rc.cfg.sig) = 8289a6d410b542f6c41a08bcfe8473aa
MD5 (V01.03.0700_Goggles_dji_system/wm220_gl.cfg.sig) = 072e68d8ebbcdebbcee86b73a9f0bbd8
MD5 (V01.03.0700_Mavic_dji_system/wm220.cfg.sig) = 072e68d8ebbcdebbcee86b73a9f0bbd8
MD5 (V01.03.0700_RC_Mavic_dji_system/wm220_rc.cfg.sig) = 072e68d8ebbcdebbcee86b73a9f0bbd8
MD5 (V01.03.0800_Goggles_dji_system/wm220_gl.cfg.sig) = e7baba1ce03a2c3d9ee146006840bc8c
MD5 (V01.03.0800_Mavic_dji_system/wm220.cfg.sig) = e7baba1ce03a2c3d9ee146006840bc8c
MD5 (V01.03.0800_RC_Mavic_dji_system/wm220_rc.cfg.sig) = e7baba1ce03a2c3d9ee146006840bc8c
MD5 (V01.03.0900_Goggles_dji_system/wm220_gl.cfg.sig) = efe50ff0ad3d5eb49dc2691cd066fe0e
MD5 (V01.03.0900_Mavic_dji_system/wm220.cfg.sig) = efe50ff0ad3d5eb49dc2691cd066fe0e
MD5 (V01.03.0900_RC_Mavic_dji_system/wm220_rc.cfg.sig) = efe50ff0ad3d5eb49dc2691cd066fe0e
MD5 (V01.04.0602_P4P_dji_system/wm331.cfg.sig) = ad7ebd830435dfd1c2cb09c66bc9b019
MD5 (V02.00.0106_P4_dji_system/wm330.cfg.sig) = 77f7fc7d413b7574cbe86571f8a766b6
MD5 (V01.00.0100_Spark_unknown/rc002.cfg) = 0c4e8d7ae113e94a761955abaa803515

```

### List of the Modules and What they Effect

Individual .cfg.sig files can be thought of as individual sections or modules within the entire firmware.   
The naming convention is as follows: 
`<model>_<module>_<version>_<date>.fw.sig`  

#### How to use the list

The 1st value in the file name is the Model.      
The 2nd value is what the module effects.      
The following files are all related to "Camera Upgrade" for the respective model
because the second number value 0100 is the Module #.    
```
- MD5 (wm220_0100_v02.00.55.69_20161215.pro.fw.sig)
- MD5 (wm330_0100_v01.19.52.66_20160623.fw.sig)
- MD5 (wm331_0100_v01.04.15.46_20170317.pro.fw.sig)
- etc.
```

#### Model #s

|Number (first value in file name) =  Model |
|:------------------------------------------|
wm100    =  Spark
wm220    =  Mavic
wm220_gl =  Goggles 
GL200A   =  GL200A # Mavic Controller
wm330    =  P4
wm331    =  P4P
wm620    =  Inspire2

| Module # -  Models that have a file containg this Module  -  Module Function|
|:----------------------------|
0100 - P4P, P4, i2, Mavic Camera Upgrade
0101 - P4, Mavic Camera Loader Upgrade
0104 - P4P Lens_Controller Upgrade
0106 - CAMFPGA (XLNX), XiLinx CAM FPGA? 
0305 - P4, i2 FlyCtrl_Loader, Spark, Mavic FC Loader Upgrade
0306 - P4P, P4, i2 FlyCtrl, Spark, Mavic FC APP Upgrade
0400 - P4P, P4, Spark, Mavic Gimbal Upgrade
0401 - P4P, P4 Gimbal 5223#1, i2 Gimbal_ESC Upgrade
0402 - P4P, P4 Gimbal 5223 #2, i2 SSD_Controller Upgrade
0404 - FPV_Gimbal Upgrade
0500 - i2 CenterBoard Upgrade
0501 - i2 Gear_Controller Upgrade
0600 - GLB200A MCU_051_gnd Upgrade (not encrypted)
0601 - Goggles MCU_031_gls Upgrade
0603 - Goggles MCU_051_gls Upgrade
0801 - Android recovery ROM?
0802 - Modvidius ma2155 VPU firmware, "DJI_IMX377" (CMOS image sensor) firmware, Veri Silicon Hantaro Video IP encoder/decoder ?
0803 - 
0804 - "System Initialized" ?
0805 - upgrade.zip (calibration for VPS?)
0900 - P4 OFDM, P4P, i2 LightBridge Upgrade
0905 - NFZ Database (nfz.db and bfz.sig)
0907 - Mavic modem/arm/dsp/gnd/uav "upgrade file" (unencrypted)
1100 - i2 Battery_0, P4, Spark, Mavic Battery Upgrade
1101 - i2 Battery_1 Upgrade
1200 - P4, i2, Spark, Mavic ESC0 Upgrade
1201 - P4, i2, spark, Mavic ESC1 Upgrade
1202 - P4, i2, Spark, Mavic ESC2 Upgrade
1203 - P4, i2, Spark, Mavic ESC3 Upgrade
1301 - OTA.zip?
1407 - GLB200A modem/arm/dsp/gnd/uav "upgrade file" (unencrypted)
2801 - Mavic modem/arm/dsp/gnd/uav "upgrade file" (unencrypted)
2803 -  
2807 - Mavic modem/arm/dsp/gnd/uav "upgrade file" (unencrypted)

### Normal fw.sig files
```
MD5 (wm100_0305_v34.11.00.21_20161010.pro.fw.sig) = ae7b12a944e67add75cd2c4d3d24624d
MD5 (wm100_0306_v03.02.34.25_20170527.pro.fw.sig) = 8b3a583c4728e8f882b4f292a1c8b1a2
MD5 (wm100_0306_v03.02.37.20_20170615.pro.fw.sig) = 65f55c9eb416e57ba5f1904fd5b91e4c
MD5 (wm100_0400_v00.00.01.16_20170517.pro.fw.sig) = b520be939d89f6fb703070168f56fe32
MD5 (wm100_0400_v01.00.01.20_20170531.pro.fw.sig) = f1f48c74462e2e05adfc64f079c977dc
MD5 (wm100_0801_v00.00.06.42_20170530.pro.fw.sig) = 0d692987f3199e49c60d7c9efa2af8fb
MD5 (wm100_0801_v00.00.06.59_20170614.pro.fw.sig) = 43e1b6665074007c1eeccdb7e8d3ec82
MD5 (wm100_0802_v00.04.11.30_20170519.pro.fw.sig) = 909cdb7d2c1119f6206cfef93626c8b1
MD5 (wm100_0802_v00.04.11.38_20170613.pro.fw.sig) = cb46b63b80b8921aa9776fdd4061846c
MD5 (wm100_0805_v01.01.01.27_20170528.pro.fw.sig) = c61bb849d8fe0b4798a5acd615b8a72e
MD5 (wm100_0805_v01.01.01.38_20170615.pro.fw.sig) = 704a09ba9107094be6f6a155b3915ff0
MD5 (wm100_0905_v00.00.01.04_20170301.pro.fw.sig) = f32a2c31dfa37ca56e7bffb5f21d8811
MD5 (wm100_0905_v01.00.01.04_20170602.pro.fw.sig) = b320c1d99b2329ce95ff55040df71576
MD5 (wm100_1100_v01.00.00.60_20170502.pro.fw.sig) = d6556a93beb45fc6927cda157af72e1d
MD5 (wm100_1200_v01.09.00.00_20170428.pro.fw.sig) = 277d7dd372906f1533206c47a29084cd
MD5 (wm100_1201_v01.09.00.00_20170428.pro.fw.sig) = 6170a30864186a9430d00269f34ae3f9
MD5 (wm100_1202_v01.09.00.00_20170428.pro.fw.sig) = 63cb1cd05d4a3ddb5c75c3dbc3f4c06c
MD5 (wm100_1203_v01.09.00.00_20170428.pro.fw.sig) = 3033d05d839ce0acd0f70c7c3fed9f1d
MD5 (wm220_0000_v01.03.0700_20170505.pro.cfg.sig) = 072e68d8ebbcdebbcee86b73a9f0bbd8
MD5 (wm220_0100_v02.00.55.69_20161215.pro.fw.sig) = 8f72ba727e89e3a7186e4a35561790a5
MD5 (wm220_0100_v02.01.55.93_20170120.pro.fw.sig) = 620c22872b9ab773c66c2be1626568ea
MD5 (wm220_0100_v02.02.56.21_20170228.pro.fw.sig) = 9771133d4720d7fa41293f336a992b06
MD5 (wm220_0100_v02.02.56.29_20170317.pro.fw.sig) = 314644f86b5ecd475c7a0c570693256b
MD5 (wm220_0100_v02.03.56.42_20170525.pro.fw.sig) = 3da24ca86323fa95695d1a5e37556e34
MD5 (wm220_0100_v02.03.56.43_20170615.pro.fw.sig) = d2f427f10112f8b2d56c4c74e2b7f524
MD5 (wm220_0100_v02.04.03.85_20161222_ca02.pro.fw.sig) = 4c490d2c11d478bf92fdf82bc29fef6d
MD5 (wm220_0100_v02.05.04.34_20170209_ca02.pro.fw.sig) = ea1fa2d3987c792f561a2e546bd835d4
MD5 (wm220_0100_v02.06.04.84_20170324_ca02.pro.fw.sig) = c0fb136c054e9105cff3f0cfc2b4c740
MD5 (wm220_0100_v02.07.04.98_20170520_ca02.pro.fw.sig) = b32b15a65987df6b6a0e862d4f280982
MD5 (wm220_0100_v02.07.04.99_20170613_ca02.pro.fw.sig) = 990cb85ebeb8771faf22e55ba0337ed5
MD5 (wm220_0101_v02.00.55.69_20161215.pro.fw.sig) = cff95060e9d6e24e48e790e9e8928b81
MD5 (wm220_0101_v02.01.55.93_20170120.pro.fw.sig) = fdcfc4622217fbab99aa0b82921561cd
MD5 (wm220_0101_v02.02.56.21_20170228.pro.fw.sig) = 0ba2dc61895d0b6945626491bd033a28
MD5 (wm220_0101_v02.02.56.29_20170317.pro.fw.sig) = 4c877d5b5c7e90ac70bd7873dfb31395
MD5 (wm220_0101_v02.03.56.42_20170525.pro.fw.sig) = 0269a28cb02dca8d3d6d6f571b4f8fa0
MD5 (wm220_0101_v02.03.56.43_20170615.pro.fw.sig) = 0a63f46aeee98722fec6c7332196ae5e
MD5 (wm220_0101_v02.04.03.85_20161222_ca02.pro.fw.sig) = 7150033a80893bd4551bb7a98ebbb511
MD5 (wm220_0101_v02.05.04.34_20170209_ca02.pro.fw.sig) = 8ecb557c234ad537a4b1d8b0d23fff26
MD5 (wm220_0101_v02.06.04.84_20170324_ca02.pro.fw.sig) = 6e829f457d00ab3dee6c092ca4e796c7
MD5 (wm220_0101_v02.07.04.98_20170520_ca02.pro.fw.sig) = ea28b92e89376b1f0d591c3c6a6b210e
MD5 (wm220_0101_v02.07.04.99_20170613_ca02.pro.fw.sig) = 70614bc2a2fb4ae0f35660dce008d97f
MD5 (wm220_0305_v34.04.00.23_20161122.pro.fw.sig) = c6fabddc843a0d9e6a6dd8f3c367add4
MD5 (wm220_0306_v03.02.13.12_20161209.pro.fw.sig) = 00c163103ac73e87924655a62a10484d
MD5 (wm220_0306_v03.02.13.16_20170112.pro.fw.sig) = 4371f8caf0e17c79fc3158d5f76e5737
MD5 (wm220_0306_v03.02.21.19_20170301.pro.fw.sig) = 06ac667d3d2cfd885702dca0a33b8284
MD5 (wm220_0306_v03.02.21.31_20170402.pro.fw.sig) = ce8e53632786ca555fcbe7c483d71309
MD5 (wm220_0306_v03.02.30.13_20170405.pro.fw.sig) = 61df5e5a394c00cc50e04044597ba22d
MD5 (wm220_0306_v03.02.35.05_20170525.pro.fw.sig) = de52c171a97b6735d5f8fa867b426f35
MD5 (wm220_0400_v01.50.11.91_20161217.pro.fw.sig) = 257ec18d7a0755d084647088ec284710
MD5 (wm220_0400_v01.50.11.93_20170116.pro.fw.sig) = 947ba404517e3e9f2bcc47a80ff02d75
MD5 (wm220_0400_v01.50.11.94_20170217.pro.fw.sig) = 5add4474ca258367be7fbf6f9f3f4b04
MD5 (wm220_0400_v01.50.11.99_20170407.pro.fw.sig) = a9cd17fa3fbfc37d12f27158f5e83121
MD5 (wm220_0400_v01.50.12.01_20170414.pro.fw.sig) = ee50707d32802cb540a6ade646f1ee35
MD5 (wm220_0400_v01.50.12.05_20170523.pro.fw.sig) = 2bb6df2b17fdae49c366f07a00cc28cc
MD5 (wm220_0600_v00.00.01.27_20161017.pro.fw.sig) = 2f80ec7ebe0c7b02f356f15471e14bea
MD5 (wm220_0601_v00.00.03.04_20170329.pro.fw.sig) = 31d9ba179ac8c8f22b5e7079258bbfc0
MD5 (wm220_0601_v00.00.03.05_20170527.pro.fw.sig) = 75f16f8552f8919b5de288303382500f
MD5 (wm220_0603_v00.00.06.07_20170314.pro.fw.sig) = afe9d32ba93a118a3fefbb2ce4b3850a
MD5 (wm220_0603_v00.00.06.08_20170519.pro.fw.sig) = e1d2e415ae193b8f05b684ef42308a37
MD5 (wm220_0801_v01.03.12.04_20161222.pro.fw.sig) = 48b4a0f7497088275ae1214e8f970e97
MD5 (wm220_0801_v01.04.17.03_20170120.pro.fw.sig) = e0566f2fd5c14ddf7aa234b94ef503d4
MD5 (wm220_0801_v01.05.00.08_20170227.pro.fw.sig) = 01b724fdc4cd6d03ac23be3828403f06
MD5 (wm220_0801_v01.05.00.20_20170331.pro.fw.sig) = a79d46134779a73cb7cc4ae687f8e6a4
MD5 (wm220_0801_v01.05.01.07_20170601.pro.fw.sig) = d78c07b087fc65a5ef3eb59aed3fe281
MD5 (wm220_0801_v01.05.02.08_20170619.pro.fw.sig) = 797f3b4cec7cb749066b8311ab9408de
MD5 (wm220_0802_v01.00.03.05_20161130.pro.fw.sig) = ab0841872c6ccaf9723a02cba41ae983
MD5 (wm220_0802_v01.00.03.08_20170116.pro.fw.sig) = a946c3e153ae232fa2f96141524ba7f9
MD5 (wm220_0802_v01.01.00.01_20170519.pro.fw.sig) = ec9f0466a683db8a3b36a7f23abbbed3
MD5 (wm220_0803_v00.00.04.06_20160621.pro.fw.sig) = 549d2cd141e8afff330596c790cf67aa
MD5 (wm220_0803_v00.00.04.08_20170314.pro.fw.sig) = 31065bb04b6a1062a7cbf0409455dc97
MD5 (wm220_0804_v01.00.00.04_20161107.pro.fw.sig) = aec2b905969c43284a076d7165b37340
MD5 (wm220_0804_v01.00.00.08_20170113.pro.fw.sig) = 0d7186a5caea88c82a4a78b9a8f0447c
MD5 (wm220_0805_v01.01.00.68_20161216.pro.fw.sig) = c00b0164e7c936bfb0c2ccede3bfffac
MD5 (wm220_0805_v01.01.00.71_20161227.pro.fw.sig) = 8ef3d1d412a0e6b65542654ed8cf7c94
MD5 (wm220_0805_v01.01.00.78_20170221.pro.fw.sig) = a9ddb290151e9f59ebe1d286625a11f0
MD5 (wm220_0805_v01.01.00.85_20170406.pro.fw.sig) = 96a69d18b49e3f13e38761bc0a225c27
MD5 (wm220_0805_v01.01.00.87_20170427.pro.fw.sig) = 6fa120e403c383118b35d95bd9f85d88
MD5 (wm220_0805_v01.01.00.92_20170523.pro.fw.sig) = 414b309fd107092e3a3579075e3deca6
MD5 (wm220_0805_v01.01.00.94_20170614.pro.fw.sig) = 08e4d672014de67b79d216d89be221d6
MD5 (wm220_0905_v00.00.01.04_20170301.pro.fw.sig) = 221c6661b5c60afb04fa32335815f470
MD5 (wm220_0905_v01.00.01.04_20170527.pro.fw.sig) = c29b7bcfd612ffa6996840678dcc4c86
MD5 (wm220_0907_v43.97.02.02_20161209.pro.fw.sig) = 176753d36cdf390721172f4bfc04e94b
MD5 (wm220_0907_v43.97.02.05_20170111.pro.fw.sig) = 7e9212b9ec68ca8e9600be28a9a69cd3
MD5 (wm220_0907_v47.26.02.08_20170309.pro.fw.sig) = 0adfd2e97b6a73b05dc20b7b5edbe836
MD5 (wm220_0907_v47.26.02.11_20170419.pro.fw.sig) = 4c393f76d69db509098a561f3fed6c30
MD5 (wm220_0907_v47.26.02.12_20170519.pro.fw.sig) = d5b505aa4f76bdde40e001d80e81186b
MD5 (wm220_0907_v47.26.02.14_20170613.pro.fw.sig) = 81cfd406bf77522b83e20721bac493bd
MD5 (wm220_1100_v01.00.07.24_20161206.pro.fw.sig) = 25c48c458c4a39d0bb556a3c9085b073
MD5 (wm220_1100_v01.00.07.31_20170516.pro.fw.sig) = 10b64526c2a0252718e7862c60a95a34
MD5 (wm220_1200_v01.08.00.01_20160705.pro.fw.sig) = 10c7d185ddd41b2005bae0fba6aa332a
MD5 (wm220_1200_v01.09.00.00_20161204.pro.fw.sig) = f8b0eb9ce619161a7a356a080d58915e
MD5 (wm220_1201_v01.08.00.01_20160705.pro.fw.sig) = 07f47b970ce7ff20d20f853ab72c6caf
MD5 (wm220_1201_v01.09.00.00_20161204.pro.fw.sig) = e0615c4437c221741cd88ec045750668
MD5 (wm220_1202_v01.08.00.01_20160705.pro.fw.sig) = c4bbc87abee6550adae92bc096fe7553
MD5 (wm220_1202_v01.09.00.00_20161204.pro.fw.sig) = 38dc6ef9da92998658ae942ecaae8839
MD5 (wm220_1203_v01.08.00.01_20160705.pro.fw.sig) = 999ef2b2a2f27829d6b1935fca84eca0
MD5 (wm220_1203_v01.09.00.00_20161204.pro.fw.sig) = 104466fbeec76684683c9f9233999977
MD5 (wm220_1301_v01.03.12.04_20161222.pro.fw.sig) = 1d2b0e13cd5a13c586907bfc3daf10a3
MD5 (wm220_1301_v01.04.17.03_20170120.pro.fw.sig) = 969dfe5b2a69daee7c2be60338257212
MD5 (wm220_1301_v01.05.00.08_20170227.pro.fw.sig) = 0260b5fb6cea0575153454e2e8b56d6b
MD5 (wm220_1301_v01.05.00.20_20170331.pro.fw.sig) = bee74430243d4c69743f4abef6574718
MD5 (wm220_1301_v01.05.00.23_20170418.pro.fw.sig) = 65d3e2dcf78b6e41137e17e106b0424f
MD5 (wm220_1301_v01.05.01.07_20170601.pro.fw.sig) = 92bdba7e212f445614a84514f0647fea
MD5 (wm220_1301_v01.05.02.08_20170619.pro.fw.sig) = 725bec619fe6d9553b9b594ef4bd0756
MD5 (wm220_1407_v43.97.02.02_20161209.pro.fw.sig) = 61b97ad2fb4850462dace0ff149421d7
MD5 (wm220_1407_v43.97.02.05_20170111.pro.fw.sig) = 04c04755862b5ca64bf9a4d59b6e8324
MD5 (wm220_1407_v47.26.02.08_20170309.pro.fw.sig) = b07f1dc903d5695e0c0e48f5914c73cf
MD5 (wm220_1407_v47.26.02.11_20170419.pro.fw.sig) = e62c7b4a5408f271b83aa890ef70ab0b
MD5 (wm220_1407_v47.26.02.12_20170519.pro.fw.sig) = 86a6dc203585122e1c649dc0d7c854bc
MD5 (wm220_1407_v47.26.02.14_20170613.pro.fw.sig) = 40bec85b22afd73ab04f2cc3af9a4db9
MD5 (wm220_2801_v01.02.19.30_20170407.pro.fw.sig) = 9c83d96a526abb4b3ea88a40e6b82cfe
MD5 (wm220_2801_v01.02.21.01_20170421.pro.fw.sig) = 3b8ca0046c8da2b8d809723643139048
MD5 (wm220_2801_v01.02.22.08_20170601.pro.fw.sig) = 048bc7efc3c40e368992539c7dfacfef
MD5 (wm220_2801_v01.02.22.20_20170620.pro.fw.sig) = 2a75572fd257ddc902b16f3db14f1685
MD5 (wm220_2803_v00.00.03.08_20170302_cd01.pro.fw.sig) = 580f0b0e5c817893467d2e15c7570de5
MD5 (wm220_2803_v00.00.03.08_20170302_cd02.pro.fw.sig) = 31fa7d6d96383683067ba597a9872fe2
MD5 (wm220_2807_v47.26.02.08_20170309.pro.fw.sig) = e603d8b76ad2e08b501efb9c833385aa
MD5 (wm220_2807_v47.26.02.11_20170419.pro.fw.sig) = ff1d46406a8fe3df3b1a6a09aa10e6d9
MD5 (wm220_2807_v47.26.02.12_20170519.pro.fw.sig) = 50133f9f07d1fe63a386c6b76197f31f
MD5 (wm220_2807_v47.26.02.14_20170613.pro.fw.sig) = 28e0226b0c8caa49a5a9c6b24848563e
MD5 (wm220_ac_fw_v01-03-0200.cfg.sig) = 9a0e3cc7b2cddc18db2c10cd18b5c07b
MD5 (wm330_0100_v01.19.52.66_20160623.fw.sig) = 0429684f341431632970dcadf8369f25
MD5 (wm330_0101_v01.16.51.96_20160519.fw.sig) = 676525776b3653e0b8dd93cbd623ca23
MD5 (wm330_0305_v34.04.00.17_20160114.fw.sig) = ce61f47940d56a6e59e2bc731ba22160
MD5 (wm330_0306_v03.01.10.93_20160707.fw.sig) = 47ff5acad6e79458599466ad01a98df6
MD5 (wm330_0306_v03.02.35.06_20170619.pro.fw.sig) = a17f43c5744fdcc1f20d719adddc95eb
MD5 (wm330_0400_v01.50.12.69_20160902.pro.fw.sig) = 58fe085624c6db584336215e02c6eb82
MD5 (wm330_0400_v01.64.00.82_20170328.pro.fw.sig) = 257ef9a0316d658f2742d952e9d51820
MD5 (wm330_0401_v01.02.00.00_20151224.fw.sig) = f59273fbcb1997c0c1663513dff90ac0
MD5 (wm330_0402_v01.02.00.00_20151224.fw.sig) = 1d29eb600b26cea4fffef57788837cbd
MD5 (wm330_0801_v01.00.10.07_20161104.pro.fw.sig) = b2fc2ff824f1ca42972ec6e780acd9c5
MD5 (wm330_0801_v01.00.10.54_20170629.pro.fw.sig) = b7b6e7a8e9bf1c493f06a0f637946fd8
MD5 (wm330_0802_v01.00.01.27_20160802.pro.fw.sig) = 744ca81a3b3f26aefc8f93e99318272f
MD5 (wm330_0802_v02.00.00.07_20170227.pro.fw.sig) = 9a61924e2df75ea9d704bf92128b4aaa
MD5 (wm330_0803_v01.00.05.06_20160203.fw.sig) = 32b287a34d96fc78b8db9f85efdfa1f0
MD5 (wm330_0804_v01.00.03.05_20160516.fw.sig) = a437af33b06272d1b801f5ea072fa7d5
MD5 (wm330_0900_v03.01.00.01_20160422.fw.sig) = 7dbd3a94939a31c8a4a06233d60e5075
MD5 (wm330_0900_v04.01.00.00_20170510.pro.fw.sig) = 6ab1c1cfc04a40594cbbb1898475ea6e
MD5 (wm330_0905_v01.00.01.04_20170527.pro.fw.sig) = 7daba2d48c83c02397636f1d614513cc
MD5 (wm330_1100_v02.00.07.14_20161031.pro.fw.sig) = 469e6c7971283bab38aad0012c39a3c8
MD5 (wm330_1100_v02.00.07.30_20170504.pro.fw.sig) = 42acc4cae2d9ba19b5a6c343f2aed113
MD5 (wm330_1200_v01.06.00.00_20160516.fw.sig) = 6617f531929b42741f8bee178bc049f0
MD5 (wm330_1200_v01.08.00.07_20160913.pro.fw.sig) = 522b035e5ebe9a73239685f02ccd6ae0
MD5 (wm330_1201_v01.06.00.00_20160516.fw.sig) = 3385ba2147cbe3eca2d99d6cdb87cab1
MD5 (wm330_1201_v01.08.00.07_20160913.pro.fw.sig) = da18983de663689adee39cda3738ba78
MD5 (wm330_1202_v01.06.00.00_20160516.fw.sig) = 72da5b03459c3dfc74146b248c780e4b
MD5 (wm330_1202_v01.08.00.07_20160913.pro.fw.sig) = e81c78d8643e5e58d0883c828ccbe077
MD5 (wm330_1203_v01.06.00.00_20160516.fw.sig) = f00a5d40abcedb47f80a5e47f0a10a2d
MD5 (wm330_1203_v01.08.00.07_20160913.pro.fw.sig) = 0cc1acdf87bde980ad37385f2bcafe55
MD5 (wm331_0100_v01.04.15.46_20170317.pro.fw.sig) = 587827190524bd719e72c1dcaa225a00
MD5 (wm331_0104_v00.09.01.85_20161221.pro.fw.sig) = 9f4899193e67354680c1aae202271bca
MD5 (wm331_0306_v03.02.30.13_20170405.pro.fw.sig) = 909d4fdd2ccacf9e711a73f01c3b4fcf
MD5 (wm331_0400_v01.50.12.94_20170302.pro.fw.sig) = acd45097d4fcc8571b3c00313733f5c2
MD5 (wm331_0401_v01.04.04.00_20160927.pro.fw.sig) = a2f7d3fb70a135dfb62800cbef63c1bf
MD5 (wm331_0402_v01.04.04.00_20160927.pro.fw.sig) = 7a1da0f9f79e6a093a8814445e811976
MD5 (wm331_0801_v01.01.03.12_20161021.pro.fw.sig) = dc75f68f2a3287e3d60fc0a204bac600
MD5 (wm331_0801_v01.01.03.50_20170227.pro.fw.sig) = 991b466f415c77226c90958216c99128
MD5 (wm331_0801_v01.01.03.64_20170406.pro.fw.sig) = 862b6eedd2ba971f4af88a3420205a6a
MD5 (wm331_0802_v01.00.01.05_20170322.pro.fw.sig) = 5fbc33635cf993dd443aa254d5f01107
MD5 (wm331_0803_v00.00.00.07_20160913_cd01.pro.fw.sig) = f4fde1aab105edd77c850c5c9f880547
MD5 (wm331_0803_v00.00.00.07_20160913_cd02.pro.fw.sig) = f4fde1aab105edd77c850c5c9f880547
MD5 (wm331_0803_v00.00.00.07_20160913_cd03.pro.fw.sig) = f4fde1aab105edd77c850c5c9f880547
MD5 (wm331_0804_v00.00.00.05_20160927.pro.fw.sig) = 02181e73dd0f6b8cd11d4c8b5b732892
MD5 (wm331_0805_v01.01.00.92_20170410.pro.fw.sig) = eef4bc038cf0615d93ac0d6c13f81334
MD5 (wm331_0900_v01.02.04.00_20170117.pro.fw.sig) = be1a09d05dc05d7bfc4ea1c5d2b6bd4a
MD5 (wm331_0905_v00.00.01.04_20170301.pro.fw.sig) = 01d1cfb3a2986330cd19705670c99336
MD5 (wm331_1100_v02.00.07.27_20170220.pro.fw.sig) = 3b18ca76e1e6861fe728e153851d4317
MD5 (wm331_1200_v01.08.00.07_20160914.pro.fw.sig) = 6ba4a754e3d05d5c61e6138bc9518134
MD5 (wm331_1201_v01.08.00.07_20160914.pro.fw.sig) = ca6dc7e1fd0158cad85c7631f135a7a2
MD5 (wm331_1202_v01.08.00.07_20160914.pro.fw.sig) = 766b0755a1ed1160538d31b5420f3217
MD5 (wm331_1203_v01.08.00.07_20160914.pro.fw.sig) = 9f4aef64c6d94eda0f1b718cdd80351e
MD5 (wm620_0100_v01.02.15.04_20170208.pro.fw.sig) = 82da811788314b0bd3152df243cab344
MD5 (wm620_0100_v01.06.15.82_20170619.pro.fw.sig) = 6f503a3a4917a9a604d3239f917a7bd0
MD5 (wm620_0104_v00.09.01.85_20161221_ln02.pro.fw.sig) = e1b335e74a6b14e1d3aca5398ba12056
MD5 (wm620_0104_v00.10.01.73_20161212_ln01.pro.fw.sig) = 7e79daa82dad2ec26cdf1f0ea59d2946
MD5 (wm620_0104_v00.12.02.24_20170531_ln01.pro.fw.sig) = e0d50421a5637313724e0d3d1fe488ca
MD5 (wm620_0106_v01.32.49.98_20170207.pro.fw.sig) = 934c4a49003a38ba14215cd6af1e4eb1
MD5 (wm620_0106_v01.37.51.00_20170620.pro.fw.sig) = d98ccd07e0842cb33600fc7f7e600c77
MD5 (wm620_0305_v34.10.00.21_20160621.pro.fw.sig) = 657cce254934bf22cb6178da959d7446
MD5 (wm620_0306_v03.02.21.19_20170301.pro.fw.sig) = 17159d4a32ebd6ada547187370b935a4
MD5 (wm620_0306_v03.02.30.13_20170405.pro.fw.sig) = 3c9bf2dacc0096c48aec2c3abe874669
MD5 (wm620_0306_v03.02.35.05_20170525.pro.fw.sig) = 04a5bc9be9a24309ba5a9bc8c14b3f82
MD5 (wm620_0400_v01.00.00.28_20170217_gb02.pro.fw.sig) = 31c536d942f747f9e82ac3da9b0af23a
MD5 (wm620_0400_v01.00.00.32_20170329_gb02.pro.fw.sig) = 74c019d31bc41ff117c5190e4b6b5b6f
MD5 (wm620_0400_v01.00.00.71_20170217_gb01.pro.fw.sig) = 479c34a270a6ce53051c2f4042cd6a44
MD5 (wm620_0400_v01.00.00.76_20170329_gb01.pro.fw.sig) = 73a410c351c75fd6906925c8384cca2e
MD5 (wm620_0400_v01.00.00.77_20170410_gb01.pro.fw.sig) = 1f2011184c28aaa6a03ba25b033ffc28
MD5 (wm620_0401_v01.06.17.17_20170206.pro.fw.sig) = 4f50851dbfa3417c1a0c3d9ed496209c
MD5 (wm620_0401_v01.06.18.17_20170324.pro.fw.sig) = 1dc00cafbdbc231608556ad010e360ac
MD5 (wm620_0401_v01.06.19.17_20170510.pro.fw.sig) = 130ab4dbae3716f8010a85415324f940
MD5 (wm620_0404_v00.00.00.27_20170126.pro.fw.sig) = 82a8ec1abb906e6ef76db896afd10ab8
MD5 (wm620_0500_v01.00.01.11_20170302.pro.fw.sig) = b7cf6fd22e6a9194b60cb33a197132ed
MD5 (wm620_0500_v01.00.01.15_20170426.pro.fw.sig) = b78a11ca8ddaa6d92966833902c270f3
MD5 (wm620_0501_v00.01.00.09_20160805.pro.fw.sig) = 3fe965bfc3a97b0d2b52523595689cf9
MD5 (wm620_0801_v01.00.00.49_20170309.pro.fw.sig) = da545044c3d0f13c46d46fcbc420bfb6
MD5 (wm620_0801_v01.00.00.55_20170402.pro.fw.sig) = e45d146fd2392d060d9801f704637e6b
MD5 (wm620_0801_v01.00.00.82_20170601.pro.fw.sig) = cded97dfb97d4f7e2ba9a1572fac59b8
MD5 (wm620_0802_v00.00.09.06_20170113.pro.fw.sig) = 602ecb6370f61ab073a15cc2501d45bb
MD5 (wm620_0802_v00.02.00.00_20170522.pro.fw.sig) = 8156f82e42f4db1dc5d0580431fbf5f5
MD5 (wm620_0803_v00.00.02.01_20160616.pro.fw.sig) = f8ce1bebefb4c0adc1df210ecec0984c
MD5 (wm620_0803_v00.00.02.02_20170309.pro.fw.sig) = 50aeadd2c6a4117b34de44433a6278e3
MD5 (wm620_0803_v00.00.02.03_20170417.pro.fw.sig) = fc0fcd25f58e28c2b4372e9e1765fc1d
MD5 (wm620_0804_v00.01.02.05_20161103.pro.fw.sig) = 5bf0654fe74b5d2548f481e66dcc0b52
MD5 (wm620_0805_v01.01.00.63_20170210.pro.fw.sig) = 76a27c41064fc99af20e93f0783d666a
MD5 (wm620_0805_v01.01.00.65_20170317.pro.fw.sig) = 3770209b8b9db81d3e1643a551d182f2
MD5 (wm620_0805_v01.01.00.74_20170612.pro.fw.sig) = 5bcb1af3ddb304eaffb655dd434accc4
MD5 (wm620_0900_v01.02.04.00_20170117.pro.fw.sig) = a90c4f7c6feb82fb3919d46c1cfffa5b
MD5 (wm620_0900_v01.06.00.00_20170608.pro.fw.sig) = 8d7fa3d713316e6a59ae73ca694d376e
MD5 (wm620_0905_v00.00.01.04_20170301.pro.fw.sig) = 82ce95475728151328258d7d3516b9c4
MD5 (wm620_0905_v01.00.01.04_20170527.pro.fw.sig) = 43ffc5555103d1306dc3cca0c3782353
MD5 (wm620_1100_v01.00.00.35_20161220.pro.fw.sig) = 8d8ff613a68f28143fd1589ce7469ebe
MD5 (wm620_1100_v01.00.00.41_20170415.pro.fw.sig) = 741d936f7a060728c4aa68d743c3a0df
MD5 (wm620_1101_v01.00.00.35_20161220.pro.fw.sig) = fa9c8211128c0d24373b4151955e3301
MD5 (wm620_1101_v01.00.00.41_20170415.pro.fw.sig) = c8a5a06742d9f5d4e422cea3caac61db
MD5 (wm620_1200_v01.02.00.46_20160918.pro.fw.sig) = 91cef3114e5e01195ee493358a663348
MD5 (wm620_1201_v01.02.00.46_20160918.pro.fw.sig) = f3c309a0b3fa0c21e06760058abdfd30
MD5 (wm620_1202_v01.02.00.46_20160918.pro.fw.sig) = 7724e4f5b8015d6e7ead4ca063f60b1e
MD5 (wm620_1203_v01.02.00.46_20160918.pro.fw.sig) = 2a16823283b4921d84030c94599eef4d
```

### #DeejayeyeHackingClub information repos aka "The OG's" (Original Gangsters)

http://dji.retroroms.info/ - "Wiki"

https://github.com/fvantienen/dji_rev - This repository contains tools for reverse engineering DJI product firmware images.

https://github.com/Bin4ry/deejayeye-modder - APK "tweaks" for settings & "mods" for additional / altered functionality

https://github.com/hdnes/pyduml - Assistant-less firmware pushes and DUMLHacks referred to as DUMBHerring when used with "fireworks.tar" from RedHerring. DJI silently changes Assistant? great... we will just stop using it.

https://github.com/MAVProxyUser/P0VsRedHerring - RedHerring, aka "July 4th Independence Day exploit", "FTPD directory transversal 0day", etc. (Requires Assistant). We all needed a public root exploit... why not burn some 0day?

https://github.com/MAVProxyUser/dji_system.bin - Current Archive of dji_system.bin files that compose firmware updates referenced by MD5 sum. These can be used to upgrade and downgrade, and root your I2, P4, Mavic, Spark, Goggles, and Mavic RC to your hearts content. (Use with pyduml or DUMLDore)

https://github.com/MAVProxyUser/firm_cache - Extracted contents of dji_system.bin, in the future will be used to mix and match pieces of firmware for custom upgrade files. This repo was previously private... it is now open.

https://github.com/MAVProxyUser/DUMLrub - Ruby port of PyDUML, and firmware cherry picking tool. Allows rolling of custom firmware images.

https://github.com/jezzab/DUMLdore - Even windows users need some love, so DUMLDore was created to help archive, and flash dji_system.bin files on windows platforms.

