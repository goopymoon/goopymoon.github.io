Required tools
* [MikuMikuDance](http://www.geocities.jp/higuchuu4)
  * https://www.youtube.com/watch?v=eRp2dYzQVJs
  * https://www.youtube.com/watch?v=pAGT9pD_3Jg
  * https://www.youtube.com/watch?v=UX4II4sy1IQ
* [MMD4Mecanim](http://stereoarts.jp/)
  * pmx2fbx.exe is in the Unity package.
* [MMDBridge](https://sites.google.com/a/render.jp/mmdbridge/)
* [MikuMikuMoving](https://sites.google.com/site/mikumikumoving/)
* [Blender_mmd_tools](https://github.com/sugiany/blender_mmd_tools)
* [MMD周辺ライブラリ](https://archive.fo/DrEcB)
* [Vocaloid by Yamaha](http://www.vocaloid.com/)
* [歌声合成ツールUTAU](http://utau-synth.com/)
  
Assets
* https://bowlroll.net/file/4576
* https://soundcloud.com/
* http://kasaneteto.jp/index_ent.html

Tutorial
* [![MMD tutorial with English subs 1](https://github.com/goopymoon/goopymoon.github.io/blob/master/Image/miku_bone.PNG)](http://youtube.com/watch?v=Jx1qLlbtCQI?t=0s) 
* [MMD tutorial with English subs 2](http://youtube.com/watch?v=sCnX0EflenE)
* [3D初心者が作ったMikuMikuDance初心者向け講座](http://www.nicovideo.jp/mylist/7374894)
* [Blender](http://hellamerdurial.blogspot.com/2014/02/mmd-blender.html)
* https://creator.game.cyberagent.co.jp/

Engine Integration
* MMD Internals
  * [PMD](http://mikumikudance.wikia.com/wiki/MMD:Polygon_Model_Data) / [PMX](http://aicdg.com/oldblog/html5/2017/08/16/pmx-format.html) file format
  * VMD file format [memo](https://blog.goo.ne.jp/torisu_tetosuki/e/bc9f1c4d597341b394bd02b64597499d)/[memo 2](https://blog.goo.ne.jp/torisu_tetosuki/e/2a2cb5c2de7563c5e6f20b19e1fe6139)
  * [sph/spa file](https://learnmmd.com/http:/learnmmd.com/pmd-editor-basics-sph-and-spa-files-add-sparkle/)
  * [Rigging](https://www.deviantart.com/mmdyesbutterfly/art/PMD-Xeditor-Rigging-Tutorial-328125378)
  * [Rigid body](https://www.deviantart.com/doremi391/art/MMD-How-to-make-physics-and-joints-TUTORIAL-448716016)
  * [Joints](https://orig00.deviantart.net/7ce0/f/2017/274/9/b/pmxe_joints_stuff_by_steeldolls-dbp63or.png)
* Open GL
  * [libmmd](https://github.com/itsuhane/libmmd)
  * [Saba_viewer](https://github.com/benikabocha/saba)
    * https://qiita.com/benikabocha/items/ae9d48e314f51746f453
    * I think this is the most perfect open source code of mmd.
    * ![](https://github.com/goopymoon/goopymoon.github.io/blob/master/Image/saba_viewer.PNG)
    * How to run in debug mode in MacOS 
      * Bullet which is installed by brew has crash problem in Debug mode.
      * To bypass this issue build bullet as following.
        1. comment out SIMD related definition in btScalar.h
          * https://pybullet.org/Bullet/phpBB3/viewtopic.php?t=9443
        2. Build Bullet without double precision and link this.
          * cmake -DBUILD_PYBULLET=ON -DBUILD_PYBULLET_NUMPY=ON -DUSE_DOUBLE_PRECISION=OFF -DBT_USE_EGL=ON -DCMAKE_BUILD_TYPE=Release -DCMAKE_INSTALL_PREFIX="your installation path" ..
* Unity
  * [MMD 4 Unity Tutorial](https://laboratoriesx86.wordpress.com/2015/04/26/tutorial-mmd-4-unity/)
  * [유니티에서 MMD 사용해보기](https://www.slideshare.net/flashscope/mmd-unity1)
    * [MMD for Unity](http://mmd-for-unity-proj.github.io/mmd-for-unity/)
      * Source code is available.
      * Physics does not work well.
      * Something wrong with transparent material
      * I made a pullrequest of upgrad to Unity2017.
    * [mmdlib-for-unity](https://github.com/goopymoon/libmmd-for-unity)
      * Source code is available.
      * Uses Bullet physics (crashes at second run. End vertex movement of skirt is weird)
      * Shader is good as MMD4Mecanim
    * [MMD4Mecanim](http://stereoarts.jp/)
      * No source code is available.
      * Perfectly imported
      * ![](https://github.com/goopymoon/goopymoon.github.io/blob/master/Image/screen_300x600_2018-09-14_00-23-13.png)
      * https://www.youtube.com/watch?v=-frQQF_y7Ps
  * [UnityにMMDモデルを取り込んでhololensで表示する](http://bluebirdofoz.hatenablog.com/entry/2017/06/11/203859)
* UE4
  * [언리얼에 MMD 불러오기](http://blog.naver.com/PostView.nhn?blogId=lsb522&logNo=220943266529)
  * [UnityChanLive UE4 Ver](https://dev.to/shop_0761/unity-chan-live-for-unrealengine-4-12l)
  * Using IM4U
    * [UE4 MMDのPMXとVMDを直接インポートし、マテリアル、IK、物理、表情モーフを一発でUE4へ持ってくる方法](http://unrealengine.hatenablog.com/entry/2016/01/11/224331)
    * [Unreal Engine4でMMDモデルに表情を付ける方法](https://creator.game.cyberagent.co.jp/?p=3798)
      * [IM4U Plugin](https://github.com/goopymoon/UnrealEngine_IM4UPlugin) - Original plugin's development is discontinued. I made a patch for version 4.20.1 in my forked repository. 
        * ![](https://github.com/goopymoon/goopymoon.github.io/blob/master/Image/tda_ue4_subsurface.PNG)
        * Automatically generated material do not have cartoon effects those originally exist.
        * Unlike pmx (pmx is UTF16 or UTF8) vmd file is shift-jis format. This cause problem during mapping bone names if locale of Windows OS is not Japanese. This is the reason why vmd import works well only in Japanese Windows.
          * Plugin's encoding helper uses MultiByteToWideChar() and WideCharToMultiByte(). These are available in all Windows versions, but the PC should contain code page 932.
          * MMD4Mecanim bypass this problem by using english bone name of VMD file.
      * [MMDBridge](https://github.com/uimac/mmdbridge) - System locale must be Japanese if bone name contains Japanese.
        * The encoding problem of Japanese bone name
          * [Normal in Japanese Windows](https://github.com/goopymoon/goopymoon.github.io/blob/master/Image/bone_name_mismatch_in_japan_locale.PNG)
          * [Abnormal in Korean Windows](https://github.com/goopymoon/goopymoon.github.io/blob/master/Image/bone_name_mismatch_in_korean_locale.PNG)
        * [View imported animation sequence in UE4](https://youtu.be/3X3dV2_NwwU)
  * Using pmx2fbx 
    * [Unreal Engine4でMMDモデルを使ってみた（前編）](https://creator.game.cyberagent.co.jp/?p=3794)
      * Material must be handled mannually according to generated model_name.xml file. cartoon effect must be considered too.
      * Morph target information is missing
    * [Unreal Engine4でMMDモデルを使ってみた（後編）](https://creator.game.cyberagent.co.jp/?p=3795)
    * [Unreal Engine4でMMDモデルをVRで見てみた](https://creator.game.cyberagent.co.jp/?p=3916)
  * Using Bledner & mmd tools
    * [The beginer's guide to Blender](https://www.blenderhd.com/wp-content/uploads/2015/08/BeginnersGuideToBlender.pdf)
    * [MMD to Blender tutorial](https://www.deviantart.com/crazy4anime09/art/MMD-to-Blender-2-79-Tutorial-718326270)
    * [MMD in Blender basic posing tutorial](https://www.deviantart.com/crazy4anime09/art/MMD-in-Blender-Basic-Posing-Tutorial-589157109)
    * [MMD in Blender importing motion tutorial](https://www.deviantart.com/crazy4anime09/art/MMD-in-Blender-Importing-Motions-Tutorial-650932100)
    * To Import motion file properly do as following steps
      * Select the bone and choose "Pose Mdoe"
      * Select the root bone then import VMD file.
      * Go to Object Mode, Select model, then import VMD for the facial
    * Fbx exported by Blender have import problem in UE4 4.20.1 such as duplicated bone name and multiple root.

Shader
* https://github.com/ray-cast/ray-mmd

Pseudo hologram
* [Unity hologram pyramid](https://assetstore.unity.com/packages/tools/hologram-pyramid-61735)
  * [DIY-Pyramid-Hologram](https://www.instructables.com/id/DIY-Pyramid-Hologram/)
  * [![MMD multi-projection](https://github.com/goopymoon/goopymoon.github.io/blob/master/Image/miku_hologram.PNG)](https://www.youtube.com/watch?v=-frQQF_y7Ps?t=0s) [![MMD hologram](http://img.youtube.com/vi/FUwaFAuOZmg/0.jpg)](https://youtu.be/FUwaFAuOZmg?t=0s)
* [Hologram looking glass](https://m.post.naver.com/viewer/postView.nhn?volumeNo=16377390&memberNo=29546687&vType=VERTICAL)
* [Gatebox](https://gatebox.ai/home/)
* [Opengl on raspberry pi](http://www.raspberryconnect.com/gamessoftware/item/314-trying_out_opengl_on_raspberry_pi_3)
* [Raspberry pi pocket projector](https://www.raspberrypi.org/blog/build-raspberry-pi-pocket-projector/)

ARKit
* https://blendersushi.blogspot.com/2017/08/arkit-blender-mikumikudance-mmd-for.html

