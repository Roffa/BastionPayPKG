# BastionPayPKG
建立IPA在线下载

1. 通过公司账号打包生成IPA文件
2. https://zc.pgyer.com 使用此链接将IPA重签为企业证书（需要付费，还不便宜）
3. 由于区块链项目，不允许在上面平台直接上架，需要自建分发平台,可直接上架的，无需看下面内容
4. 在GitHub上新建一个项目（选择分发平台为GitHub）
5. clone项目到本地,在本地路径中增加57*57、512*512 icon, 增加已经重签完毕的IPA包，增加manifest.plist文件
6. push本地更新到Github,在Github上获取到本地更新文件的下载地址。（进入文件，右击下载按钮，copy链接）
7. 在manifest文件中修改57*57下载链接、512*512下载链接、IPA下载链接为对应的有效链接
8. 上面已经提级到manifest.plist文件的地址，其实安装地址格式为:
itms-services://?action=download-manifest&url=上面所获取的plist地址
示例如下:
itms-services://?action=download-manifest&url=https://raw.githubusercontent.com/******/******/master/manifest.plist
9. 用Safari打开上面地址实现安装


￼
