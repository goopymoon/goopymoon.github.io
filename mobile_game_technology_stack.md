Unreal
* [C++11~](https://github.com/jwvg0425/ModernCppStudy/wiki)
* [Coding Style](https://docs.unrealengine.com/latest/INT/Programming/Development/CodingStandard/index.html)
* [UnrealVS Setup](http://api.unrealengine.com/KOR/Programming/Development/VisualStudioSetup/UnrealVS/index.html)
* Installedbuild: how to use [UAT](https://blog.mi.hdm-stuttgart.de/index.php/2017/02/11/uat-automation/)
  * Making installedbuild in terminal
    * EnginePath/Build/BatchFiles/RunUAT.bat BuildGraph -target="Make Installed Build Win64" -script=EnginePath/Build/InstalledEngineBuild.xml -set:WithWin64=true -set:WithAndroid=true -set:WithWin32=false -set:WithLinux=false -set:WithLumin=false
  * Making apk in terminal
    * EnginePath/Build/BatchFiles/RunUAT.bat BuildCookRun -Project=ProjectName.uproject -NoP4 -TargetPlatform=Android_ASTC -Platform=Android -ClientConfig=Development -Cook -allMaps -Build -Stage -Pak -Archive -ArchiveDirectory=OutputPath -Rocket -Package

* [Android debugging](http://pafuhana1213.hatenablog.com/entry/2018/02/15/001307)
* [commandlet](https://api.unrealengine.com/udk/Three/CommandletHome.html)
* [UE4 Network Compendium](http://cedric-neukirchen.net/Downloads/Compendium/UE4_Network_Compendium_by_Cedric_eXi_Neukirchen.pdf)
* [Test Automation](https://docs.unrealengine.com/en-us/Programming/Automation/TechnicalGuide)
* [CSM](http://api.unrealengine.com/KOR/Platforms/Mobile/Lighting/HowTo/CascadedShadow/index.html)
* [Unreal Summit 2017: ](http://replay.unrealsummit.co.kr/pp3.html)[pdf](http://replay.unrealsummit.co.kr/data2017/pp3.pdf)
* [Getting Started with VR in Unreal Engine 4](https://www.tomlooman.com/getting-started-with-vr/)
  * [Creating a VR Pawn](https://wirewhiz.com/unreal-engine/)
  * [Motion Controller Component Setup](https://docs.unrealengine.com/en-US/SharingAndReleasing/XRDevelopment/VR/DevelopVR/MotionController/index.html)
  * https://github.com/tomlooman/VRTemplates
* [Designing Blueprint Function Nodes in C++](https://mikelis.net/designing-blueprint-nodes-through-c/)

Unity
* [Using Streaming Assets in Unity](https://www.raywenderlich.com/165809/using-streaming-assets-unity), [Assetbundle fundamentals](https://unity3d.com/kr/learn/tutorials/topics/best-practices/assetbundle-fundamentals), [Resources folder](https://unity3d.com/kr/learn/tutorials/temas/best-practices/resources-folder)
* [Execution Order of Event Functions](https://docs.unity3d.com/Manual/ExecutionOrder.html)

[Graphics](https://github.com/goopymoon/goopymoon.github.io/blob/master/graphics.md)
* [Spine](http://esotericsoftware.com/), [Live2D](http://www.live2d.com/ja/)([tutorial](http://sites.cybernoids.jp/cubism2_kr/))

Gamming AI
  * [FSM vs. Behavior tree](https://web.stanford.edu/class/cs123/lectures/CS123_lec08_HFSM_BT.pdf): [2009 ndc](https://www.slideshare.net/yonghakim900/2009-ndc)
  * Behavior Tree: [Introduction](http://blog.renatopp.com/2014/07/25/an-introduction-to-behavior-trees-part-1/), [tool](https://archive.codeplex.com/?p=brainiac)
  * [Are Behavior Trees a Thing of the Past](https://www.gamasutra.com/blogs/JakobRasmussen/20160427/271188/Are_Behavior_Trees_a_Thing_of_the_Past.php)

Smart contract
* [Solidity tutorial: CrytoZombies](https://cryptozombies.io/en/course/)

Server Development Environment
* git: [branch name prompt](https://coderwall.com/p/fasnya/add-git-branch-name-to-bash-prompt), [merge vs rebase](https://www.atlassian.com/git/tutorials/merging-vs-rebasing), [fast forward](https://ariya.io/2013/09/fast-forward-git-merge)
* Logging: [log4cxx](https://logging.apache.org/log4cxx/latest_stable/), [chucho](https://github.com/mexicowilly/Chucho/wiki)
* Redis: [GUI tool](https://redisdesktop.com/), [Command](http://www.redisgate.com/redis/command/commands.php), [tips](https://redislabs.com/blog/5-key-takeaways-for-developing-with-redis/)
* Rabbitmq: [access control](https://www.rabbitmq.com/access-control.html)
* Lua: [luarocks](https://luarocks.org/),[luacheck](https://luarocks.org/modules/mpeterv/luacheck), [CJson](https://github.com/mpx/lua-cjson)
* [Using Docker Compose](http://raccoonyy.github.io/docker-usages-for-dev-environment-setup/) + [Vagrant](https://www.vagrantup.com/docs/index.html)
* VirtualBox: [Resizing under Windows Host](http://derekmolloy.ie/resize-a-virtualbox-disk/) - You can install and run gparted in target Ubuntu. gparted does not work in Ubuntu 17.10. In this case don't forget "Before you log in, click on the gear next to login and switch to xorg".
* [Vim setting](https://bluesh55.github.io/2016/10/09/vim-ide/)
* Editor: [Atom](https://atom.io/), VSCode([Ubuntu](https://code.visualstudio.com/docs/setup/linux, [Max tip](https://code.visualstudio.com/docs/getstarted/userinterface)), [ESLint extension](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint))
* DB migration: [Ruby On Rails](http://rubyonrails.org/), [Django](https://www.djangoproject.com/) & [South](https://south.readthedocs.io/en/latest/)
* CI(Continuous Integration): [Jenkins](https://jenkins-ci.org/)

[NodeJS](https://nodejs.org/api/)
* [template literals](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Template_literals)
* http: [Status Code Definitions](https://www.w3.org/Protocols/rfc2616/rfc2616-sec10.html)
* config: [node-config](https://www.npmjs.com/package/config)
* logging: [winston](https://github.com/winstonjs/winston), [morgan](https://www.npmjs.com/package/morgan)
* utils: [lodash](https://lodash.com/)
* Validation: [validate.js](https://validatejs.org/), [Validator](https://github.com/chriso/validator.js), [express-validator](https://github.com/ctavan/express-validator), [JSON-Schema](https://code.tutsplus.com/series/validating-data-with-json-schema--cms-966)
* [JSON table schema](http://paulfitz.github.io/dataprotocols/json-table-schema/)
* Code generation: [Mustache](https://www.npmjs.com/package/mustache)
* Architecture: [promise](https://pouchdb.com/2015/05/18/we-have-a-problem-with-promises.html), [Express vs. Koa vs. Hapi](https://www.airpair.com/node.js/posts/nodejs-framework-comparison-express-koa-hapi), [Async/Await](https://dev.to/geoffdavis/writing-asyncawait-middleware-in-express-6i0)
* UI design: [React](https://reactjs.org/docs/design-principles.html) + [Redux](https://deminoth.github.io/redux/) ([http://huns.me/development/1953](http://huns.me/development/1953))
* TDD: [mocha](https://github.com/mochajs/mocha#sponsors), [Jasmine](https://github.com/jasmine/jasmine/wiki), [Mocha vs. Jasmine](https://marcofranssen.nl/jasmine-vs-mocha/)
* [ESLint](https://eslint.org/docs/user-guide/getting-started), [Airbnb JavaScript Style Guide](https://github.com/airbnb/javascript)
* [nodemon](https://nodemon.io/), [PM2](http://pm2.keymetrics.io/)([Simple Usage](https://cheese10yun.github.io/PM2/), [Process File](http://pm2.keymetrics.io/docs/usage/application-declaration/))
* [how to benchmark](https://aws.amazon.com/ko/blogs/korea/how-to-loading-test-based-on-aws/)
* [JavaScript books - free to read online](http://exploringjs.com/)

[Typescript](https://www.typescriptlang.org/docs/home.html)
* [map type](https://www.npmjs.com/package/typescript-map)
* [CRUD tutorial](http://mherman.org/blog/2016/11/05/developing-a-restful-api-with-node-and-typescript/#.WmmQFxg6-i4)
* [TypeScript 2.1: async/await for ES3/ES5](https://blog.mariusschulz.com/2016/12/09/typescript-2-1-async-await-for-es3-es5)
* [6 Reasons Why JavaScript’s Async/Await Blows Promises Away (Tutorial)](https://hackernoon.com/6-reasons-why-javascripts-async-await-blows-promises-away-tutorial-c7ec10518dd9)
* [How to handle async functions inside constructors in TypeScript](https://rostacik.net/2017/04/23/how-to-handle-async-functions-inside-constructors-in-typescript/)
* [tslint](https://spin.atomicobject.com/2017/06/05/tslint-linting-setup/)
* [how to debug ts in vscode](https://medium.com/@dupski/debug-typescript-in-vs-code-without-compiling-using-ts-node-9d1f4f9a94a)

Gaming Service Archetecture
* [Elasticsearch Service](http://docs.aws.amazon.com/ko_kr/elasticsearch-service/latest/developerguide/aes-dg.pdf)
* [Log Aggregation](https://logz.io/blog/kafka-vs-redis/) 
* [How to Use Elasticsearch, Logstash, and Kibana to Manage Redis Logs](https://qbox.io/blog/redis-logs-elasticsearch-logstash-kibana)
* [How to Install and Configure the ELK Stack on Ubuntu](http://blog.daum.net/utpark0/14)
* [How To Install and Configure Redis on Ubuntu](https://www.digitalocean.com/community/tutorials/how-to-install-and-configure-redis-on-ubuntu-16-04)
* [Enable Authentication in ElasticSearch](http://blog.raffaeu.com/archive/2016/02/17/enable-authentication-in-elasticsearch.aspx)
* [posgresql log](https://blog.2ndquadrant.com/redislog-integrating-postgresql-with-logstash-for-devops-real-time-monitoring/)
* [Deploy using Rundeck and Ansible](https://gitlab.com/alandie/Rundeck-Ansible-AWS/tree/master/Rundeck-Ansible-AWS)
* [Crash Reporting - hocketyapp](https://hockeyapp.net/)

Seminar & Webinar 
* [Cloud Gaming Architecture](https://s3-eu-west-1.amazonaws.com/aws-de-media/images/_Berlin_Loft_Slides/cloud_gaming_architectures.pdf)
* [Gaming on ASW 10/24/2017](https://github.com/goopymoon/goopymoon.github.io/blob/master/Docs/GamingOnAWS2017)
* [AWS를 활용하여 Daily Report 만들기](https://www.slideshare.net/changjej/aws-daily-report)
* [KGC 2014 가볍고 유연하게 데이터 분석하기](https://www.slideshare.net/julingks/kgc2014?next_slideshow=1)

Network
* [UE4 Networking in Advanced - Engine Source Analysis & High-Level Cases](https://dawnarc.com/2019/06/ue4networking-in-advanced-engine-source-analysis-high-level-cases/)
* http://download.enmasse.com/documents/201205-gdm-tera.pdf
* [TERA Server Architecture](https://www.slideshare.net/ujentus/cgdc2010)
* [TERA 서버의 Modern C++ 활용기](https://www.slideshare.net/sangheonlee9/ndc2016-tera-modern-c)
* [테라 한승환 팀장의 "심리스월드 서버 구현 노하우"](http://m.inven.co.kr/webzine/wznews.php?idx=60184&site=tera)
* [Destiny's network mission architecture](https://www.gdcvault.com/play/1022247/Shared-World-Shooter-Destiny-s)
* [UE4 Sockets multi-thread TCP communication](https://www.programmersought.com/article/91094430036/)
* packet loss
  * https://answers.unrealengine.com/questions/515898/network-serialization-is-sensible-to-packet-corrup.html
  * Digging into Unreal Engine 4.21 Changes
    * New: Total packets sent/received, total number of bytes sent/received, and total packets lost both in and out are now kept track in the net driver.
  * https://wiki.beyondunreal.com/Everything_you_ever_wanted_to_know_about_replication_(but_were_afraid_to_ask)#Reliability
  * https://forums.unrealengine.com/legacy-tools-unreal-engine-3-udk/udk-programming-and-unrealscript/1440415-replication-packet-loss
  * https://www.makinggames.biz/programming/a-year-of-rain-network-optimisation,2335479.html
  * https://www.gamasutra.com/blogs/GafgarDavallius/20190718/346598/Satisfactory_Network_Optimizations.php

GameLift
* [Amazon GameLift](https://docs.aws.amazon.com/ko_kr/gamelift/latest/developerguide/gamelift-intro.html)
* [How to integrate Unreal Engine with GameLift and other AWS services](https://forums.awsgametech.com/t/how-to-integrate-unreal-engine-with-gamelift-and-other-aws-services-tutorial-video-series/9096)
* [Tutorial on integrating Unreal with Amazon GameLift](https://answers.unrealengine.com/questions/884106/tutorial-on-integrating-unreal-with-amazon-gamelif.html)
  * [셈플 코드](https://github.com/zeliard/GameLift)
  * [Amazon GameLift Server SDK](https://aws.amazon.com/ko/gamelift/getting-started/#Developer_Resources)
  * [AWS SDK for C++](https://github.com/aws/aws-sdk-cpp)
* [아마존의 관리형 게임 플랫폼 활용하기: GameLift (Deep Dive)](https://www.slideshare.net/awskorea/amazon-game-lift-deep-dive-seungmo-koo/)
* https://www.epicgames.com/fortnite/en-US/news/postmortem-of-service-outage-at-3-4m-ccu?lang=en-US

Online subsystem
* [UE4のOnlineSubsystemをさわってみた](https://qiita.com/mechamogera/items/312333b165b4b9940f09)
* [EOS tutorial](https://www.youtube.com/watch?v=3u0EgoD-4YQ)

