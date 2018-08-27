Required tools
* [MikuMikuDance](http://www.geocities.jp/higuchuu4)
  * https://www.youtube.com/watch?v=eRp2dYzQVJs
  * https://www.youtube.com/watch?v=pAGT9pD_3Jg
  * https://www.youtube.com/watch?v=UX4II4sy1IQ
  * [PMX file format](https://gist.github.com/ulrikdamm/8274171)
* [MMD4Mecanim](http://stereoarts.jp/)
  * pmx2fbx.exe is in Unity the package.
* [MMDBridge](https://sites.google.com/a/render.jp/mmdbridge/)
* [MikuMikuMoving](https://sites.google.com/site/mikumikumoving/)
* [MMD周辺ライブラリ](https://archive.fo/DrEcB)
* [Vocaloid by Yamaha](http://www.vocaloid.com/)
* [歌声合成ツールUTAU](http://utau-synth.com/)

Assets
* https://bowlroll.net/file/4576
* https://soundcloud.com/
* http://kasaneteto.jp/index_ent.html

Tutorial
* [MMD tutorial with English subs 1](http://youtube.com/watch?v=Jx1qLlbtCQI)
* [MMD tutorial with English subs 2](http://youtube.com/watch?v=sCnX0EflenE)
* [3D初心者が作ったMikuMikuDance初心者向け講座](http://www.nicovideo.jp/mylist/7374894)
* [Blender](http://hellamerdurial.blogspot.com/2014/02/mmd-blender.html)
* https://creator.game.cyberagent.co.jp/

Engine Integration
* Unity
  * [MMD 4 Unity Tutorial](https://laboratoriesx86.wordpress.com/2015/04/26/tutorial-mmd-4-unity/)
  * [유니티에서 MMD 사용해보기](https://www.slideshare.net/flashscope/mmd-unity1)
* UE4
  * [언리얼에 MMD 불러오기](http://blog.naver.com/PostView.nhn?blogId=lsb522&logNo=220943266529)
  * Using IM4U
    * [UE4 MMDのPMXとVMDを直接インポートし、マテリアル、IK、物理、表情モーフを一発でUE4へ持ってくる方法](http://unrealengine.hatenablog.com/entry/2016/01/11/224331)
    * [Unreal Engine4でMMDモデルに表情を付ける方法](https://creator.game.cyberagent.co.jp/?p=3798)
      * [IM4U Plugin](https://github.com/goopymoon/UnrealEngine_IM4UPlugin) - I'm testing patch for version 4.20.1 before pull request
      * [MMDBridge](https://github.com/uimac/mmdbridge) I've fixed vmd export bug and made a pull request.
      * Automatically generated material has no cartoon effect which is originally exists.
  * Using pmx2fbx 
    * [Unreal Engine4でMMDモデルを使ってみた（前編）](https://creator.game.cyberagent.co.jp/?p=3794)
      * Material must be handled mannually according to generated model_name.xml file. cartoon effect must be considered too.
      * Morph target information is missing
    * [Unreal Engine4でMMDモデルを使ってみた（後編）](https://creator.game.cyberagent.co.jp/?p=3795)
    * [Unreal Engine4でMMDモデルをVRで見てみた](https://creator.game.cyberagent.co.jp/?p=3916)

Shader
* https://github.com/ray-cast/ray-mmd

Animation
* [Creating custom Fortnite dances with webcam and Deep Learning](https://towardsdatascience.com/creating-custom-fortnite-dances-with-webcam-and-deep-learning-9b1a236c1b59)
* [Music-Driven Dance Generation with Neural Networks](https://omid.al/projects/GrooveNet.html)
* [Sequential Deep Learning for Dancing Motion Generation](http://www.osaka-kyoiku.ac.jp/~challeng/SIG-Challenge-046/SIG-Challenge-046-08.pdf)
* [Machine-Learning Algorithm Watches Dance Dance Revolution, Then Creates Dances of Its Own](https://www.technologyreview.com/s/604000/machine-learning-algorithm-watches-dance-dance-revolution-then-creates-dances-of-its-own/)
* [Learn Audio Beat Tracking for Music Information Retrieval](https://www.analyticsvidhya.com/blog/2018/02/audio-beat-tracking-for-music-information-retrieval/)
* [Classification of K-Pop Dance Movements Based on
Skeleton Information Obtained by a Kinect Sensor](https://pdfs.semanticscholar.org/d0a1/12f02818a57f3a10364d555c8c40bdfabbcd.pdf)
* [3D Human Motion Capture from 2D Video using Cloud-Based CNNs](http://on-demand.gputechconf.com/gtc/2017/presentation/s7289-paul-kruszewski-human-motion-capture-from-2d-video-using-cloud-based-cnns.pdf)
* [Example-Guided Deep Reinforcement Learning of Physics-Based Character Skills](https://xbpeng.github.io/projects/DeepMimic/index.html)
* [A DEEP LEARNING FRAMEWORK FOR CHARACTER MOTION SYNTHESIS AND EDITING](http://www.gameanim.com/2016/05/22/deep-learning-framework-character-motion-synthesis-editing/)
  * [pdf](http://www.ipab.inf.ed.ac.uk/cgvu/motionsynthesis.pdf)
* [Recurrent Neural Networks for Modeling Motion Capture Data](https://www.eurasip.org/Proceedings/Eusipco/Eusipco2017/wpapers/DL2.pdf)
* [AI powered motion capture](https://getrad.co/)
  * https://www.forbes.com/sites/nvidia/2018/05/09/ai-powered-motion-capture-a-radical-step-toward-modern-3d-content-pipelines/#70d838d5b551
* [Monocular Human Motion Capture
using a CNN Coupled with a Geometric Prior](https://arxiv.org/pdf/1701.02354.pdf)
* [Deep Learning Dance Smackdown](http://silky.github.io/posts/2017-08-28-deep-learning-dance-smackdown.html)
