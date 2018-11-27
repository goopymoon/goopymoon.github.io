Interested in the intelligent vocaloid.

* [Graphics](https://github.com/goopymoon/goopymoon.github.io/blob/master/graphics.md)
* [Mobile game technolgy stack](https://github.com/goopymoon/goopymoon.github.io/blob/master/mobile_game_technology_stack.md)
* Gamming AI
  * [FSM vs. Behavior tree](https://web.stanford.edu/class/cs123/lectures/CS123_lec08_HFSM_BT.pdf): [2009 ndc](https://www.slideshare.net/yonghakim900/2009-ndc)
  * Behavior Tree: [Introduction](http://blog.renatopp.com/2014/07/25/an-introduction-to-behavior-trees-part-1/), [tool](https://archive.codeplex.com/?p=brainiac)
  * [Are Behavior Trees a Thing of the Past](https://www.gamasutra.com/blogs/JakobRasmussen/20160427/271188/Are_Behavior_Trees_a_Thing_of_the_Past.php)
  * [Understanding ML through the Unity's ml agent](https://docs.google.com/presentation/d/e/2PACX-1vRloM3dMgWk55xAU-0nctVsxQIE2zqt6eANo0x8fqTcrlkvzkymB5R-kOIypL3QnDid1rqF0yl4kBmV/pub?start=false&loop=false&delayms=3000)
* [Machine Learning](https://github.com/goopymoon/goopymoon.github.io/blob/master/CNN.md)
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

Motion Capture using ML
* [This Reinforcement Learning Algorithm Can Capture Motion and Recreate It](https://arxiv.org/pdf/1810.03599.pdf)
* [Creating custom Fortnite dances with webcam and Deep Learning](https://towardsdatascience.com/creating-custom-fortnite-dances-with-webcam-and-deep-learning-9b1a236c1b59)
* [Classification of K-Pop Dance Movements Based on
Skeleton Information Obtained by a Kinect Sensor](https://pdfs.semanticscholar.org/d0a1/12f02818a57f3a10364d555c8c40bdfabbcd.pdf)
* [3D Human Motion Capture from 2D Video using Cloud-Based CNNs](http://on-demand.gputechconf.com/gtc/2017/presentation/s7289-paul-kruszewski-human-motion-capture-from-2d-video-using-cloud-based-cnns.pdf)
* [Example-Guided Deep Reinforcement Learning of Physics-Based Character Skills](https://xbpeng.github.io/projects/DeepMimic/index.html)
* [AI powered motion capture](https://getrad.co/)
  * https://www.forbes.com/sites/nvidia/2018/05/09/ai-powered-motion-capture-a-radical-step-toward-modern-3d-content-pipelines/#70d838d5b551
* [Monocular Human Motion Capture
using a CNN Coupled with a Geometric Prior](https://arxiv.org/pdf/1701.02354.pdf)
* [Human motion prediction](https://github.com/una-dinosauria/human-motion-prediction)
* [Recurrent Neural Networks for Modeling Motion Capture Data](https://www.eurasip.org/Proceedings/Eusipco/Eusipco2017/wpapers/DL2.pdf)

Using CMU Motion Capture Database
* [CMU Motion Capture Database](http://mocap.cs.cmu.edu)
  * [motion data file format](http://www.dcs.shef.ac.uk/intranet/research/public/resmes/CS0111.pdf)
  * [How to convert BVH to VMD](https://github.com/powroupi/blender_mmd_tools/wiki/Tutorial:-How-to-convert-BVH-to-VMD)
    * http://www6.atwiki.jp/vpvpwiki/pages/218.html#id_8e4d9a75
      * https://github.com/esetomo/mio
  * Auto Conditioned RNN motion
    * https://www.youtube.com/watch?v=FunMxjmDIQM&feature=youtu.be?t=0s
      * https://arxiv.org/pdf/1707.05363.pdf
      * https://github.com/hjzh4/Auto-Conditioned-LSTM (tensor flow version)
      * https://github.com/papagina/Auto_Conditioned_RNN_motion (original pytorch version)
  * [A DEEP LEARNING FRAMEWORK FOR CHARACTER MOTION SYNTHESIS AND EDITING](http://www.gameanim.com/2016/05/22/deep-learning-framework-character-motion-synthesis-editing/)
    * [pdf](http://www.ipab.inf.ed.ac.uk/cgvu/motionsynthesis.pdf)
    * https://github.com/AliJalalifar/Character_Animation
  * [Lecture: RNN and autoencoder: pdf](https://www.google.co.kr/url?sa=t&rct=j&q=&esrc=s&source=web&cd=1&ved=2ahUKEwj8rNb5kuzeAhXJTLwKHbG5BKwQFjAAegQIChAC&url=https%3A%2F%2Fcanvas.stanford.edu%2Ffiles%2F1079044%2Fdownload%3Fdownload_frd%3D1&usg=AOvVaw2uZMJCvtEE6eQHGcypWqev)
  * [LSTM-autoencoder](https://github.com/iwyoo/LSTM-autoencoder)

Dancing motion generation
* [Learn Audio Beat Tracking for Music Information Retrieval](https://www.analyticsvidhya.com/blog/2018/02/audio-beat-tracking-for-music-information-retrieval/)
* [Machine-Learning Algorithm Watches Dance Dance Revolution, Then Creates Dances of Its Own](https://www.technologyreview.com/s/604000/machine-learning-algorithm-watches-dance-dance-revolution-then-creates-dances-of-its-own/)
* [Sequential Deep Learning for Dancing Motion Generation](http://www.osaka-kyoiku.ac.jp/~challeng/SIG-Challenge-046/SIG-Challenge-046-08.pdf)
* [Music-Driven Dance Generation with Neural Networks](https://omid.al/projects/GrooveNet.html)
  * [essentia](https://github.com/MTG/essentia/blob/master/src/examples/tutorial/essentia_python_tutorial.ipynb)
* https://medium.com/@kcimc/discrete-figures-7d9e9c275c47
* [Deep Learning Dance Smackdown](http://silky.github.io/posts/2017-08-28-deep-learning-dance-smackdown.html)


