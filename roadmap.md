# Roadmap
This document outlines the development roadmap for the ChaosBlade project.

## V0.1.0 Roadmap (Rlease Time: 2019.06)
This version provides a lot of java chaos experiment's features, such as cpu full load in jvm, dynamic script parsing(support java and groovy script), httpclient plugin, limits of request count and request percent about chaos effected and so on.

Features/Enhancements:
* Add subcommand for querying the hit counts of java experiments in query command(#100 )
* Add support for cpu full load in jvm process(chaosblade-exec-jvm #40 )
* Add support for limits of request count and request percent about chaos effected(chaosblade-exec-jvm #46)
* Add support for dynamic script parsing(chaosblade-exec-jvm #38)
* Add support for the Apache HttpClient component(chaosblade-exec-jvm #5)


## V0.2.0 Roadmap (Rlease Time:2019.07)
This version provides C++ chaos experiments support. The C++ executor project address: https://github.com/chaosblade-io/chaosblade-exec-cplus . In addition to this, support for RocketMQ component and dubbo group matcher are also provided.

Features/Enhancements:
* Add support for cplus executor(#137 )
* Add support for dubbo group (#118 )
* Add --port args for jvm preparation(#140 )
* Add support for stopping process experiment(#136 )
* Add support for RocketMQ component (chaosblade-exec-jvm # 62)


## V0.3.0 (Rlease Time:2019.09)
Features/Enhancements:
* Support Restful API mode calls(#68 )
* Support for specifying multiple ports in network experiments(#176 )
* Add ip matcher in network experiments(#181 )
* Specify any directory to fill disk(#169 )
* Stop process for mac(#167 )
* Support linux memory experiment(#161 )
* Support cpu percent experiment(#154 )
* Add --exception-message flag in java exception experiments(#147 )
* Enhance disk burn experiment(#200 )
* Add debug mode to locate problems that are not valid for the experiment(chaosblade-io/chaosblade-exec-jvm#75)
* Add support for jvm code cache full(chaosblade-io/chaosblade-exec-jvm#68)
* Add support for jedis experiment(chaosblade-io/chaosblade-exec-jvm#79)
* Add support for postgrelsql experiment(chaosblade-io/chaosblade-exec-jvm#74)
* Add --pid for java preparation(chaosblade-io/chaosblade-exec-jvm#67)
* Add requestpath flag for servlet experiment(chaosblade-io/chaosblade-exec-jvm#63)


## V0.4.0 (Rlease Time:2019.12)
Features/Enhancements:
* Enhance status command to support more flag to filter (#251 )
* Support to destroy experiment without uid (#239 )
* Support percent flag for disk fill experiment (#217 #241 )
* Support count limit in kill process experiment (#249 )
* Support for setting ip flag when use server start command (#246 )
* Remove sudo command when current user is equals application user (#240 )
* Support method after event processing for java experiments (chaosblade-io/chaosblade-exec-jvm#91)
* Support targe object in params for java experiments (chaosblade-io/chaosblade-exec-jvm#94)
* Support for dubbo 2.7 version for java experiments (chaosblade-io/chaosblade-exec-jvm#100)
* Support to specify any namespace to deploy for chaosblade operator (chaosblade-io/chaosblade-operator#3 )


## v0.5.0 (Rlease Time:2020.1)
Features/Enhancements:
* Support multiple ip configuration for network experiments like delay, loss, corrupt, reorder and duplicate(#294 )
* Add network packets re-ordering and corruption experiments(#293 )
* Add network packet duplication experiment(#292 )
* Support mem and disk experiments for k8s(#283 )
* Add rate and mode flags for mem load experiment (#278 )
* Exclude the peer port automatically when exclude-port flag is specified in a network experiment(#277 )
* Support --reserve flag for mem load and disk fill experiments(#270 )
* Change create request method from get to post for jvm experiments(#266 )
* Enhance the JVM return function to increase the function and operator calculation of return value(chaosblade-io/chaosblade-exec-jvm#113)


## V0.6.0 (Rlease Time:2020.5)
This version adds the Pod file IO experiments and optimizes the chaosblade operator to make it more stable. In addition, the version adds some new features and fix some bugs.

Features/Enhancements:
* Add pod file system I/O experiments (#318 )
* The killing process experiment supports signal flag (#357)
* Add force overwrite flag for network experiments (#346)
* Support port occupation expriment (#345)
* Optimize chaosblade resource state flow in k8s experiments (#336)
* Retain file handle for disk fill experiment (#325)
* Remove destroy command parameter strong checksum when not using UID (#324)
* Randomly select resources from the result set in k8s experiments (#307)
* Specify local port to kill process (#275)
* Add support for tars component (chaosblade-io/chaosblade-exec-jvm#124)
  

## V0.7.0 (Rlease Time:2020.9)
The long-awaited v0.7.0 version is released~, especially the kubernetes chaos experiment scenarios have been enhanced, and the new features are as follows:

* Support all drill scenarios of Java under kubernetes;
* Added file chaos experiment scenarios;
* Added ssh execution channel, which can remotely execute chaos experiments on the target host;
* Optimize the implementation of kubernetes scenarios, only need to deploy a chaosblade-operator pod to achieve a generall chaos experiment, add --set damonset.enable=false during installation; for the target Pod or container in the network scenarios where the network permissions or commands are missing, you can Use -set damonset.enable=true to solve;
* The kubernetes scenarios execute on-demand deployment of plug-ins, and the execution speed is greatly improved;
* There are many known bug fixes and scenarios optimization;


## v0.8.0 (Rlease Time:2020.11)
This version optimized compilation, fixes a few bugs, recover node daemonset, and increases stability.
Thanks for the contributors: @xcaspar @tiny-x @arthur657834

Features/Enhancements
* Support to prepare JVM asynchronously. (#422 )
* Improvement compile, add usage. (#423 )
* Add a parameter --url-pattern to support drop package by match a url. (chaosblade-io/chaosblade-exec-os#58 )
* SSH channel add key authorization. (chaosblade-io/chaosblade-exec-os#59 )
* Add ignore-not-found flag in process experiments. (chaosblade-io/chaosblade-exec-os#61 )
* Exclude cache in container. (chaosblade-io/chaosblade-exec-os#62 )
* Add ignore-not-found flag in process experiments. (chaosblade-io/chaosblade-exec-os#65 )
* Add qps and reconcile count configs. (chaosblade-io/chaosblade-operator#48 )
* Script support load external jar. (chaosblade-io/chaosblade-exec-jvm#138 )
* Add mongoDB plugin. (chaosblade-io/chaosblade-exec-jvm#147 )


## v0.9.0 (Rlease Time:2020.11)
This version supports regular cleaning of invalid blade crd, fixed the Java experiment destroy problem, support for compiling chaosblade-tool-arm images, and increases stability.

Features/Enhancements
* Support for build ARM chaosblade-tool images. (#441 )
* Periodically clean up invalid blade. (chaosblade-io/chaosblade-operator#53 )


## v0.10.0 (Rlease Time:2021.3)
This version supports many scenarios, including Kafka, Hbase, lettuce and more.

Features/Enhancements
* Support hbase plugin. (chaosblade-io/chaosblade-exec-jvm#154 )
* Support elasticsearch plugin. (chaosblade-io/chaosblade-exec-jvm#155 )
* Support thread increased action. (chaosblade-io/chaosblade-exec-jvm#156 )
* Support redisson. (chaosblade-io/chaosblade-exec-jvm#159 )
* Support Lettuce client & MySQL Driver 8.x. (chaosblade-io/chaosblade-exec-jvm#160 )
* Support kafka plugin. (chaosblade-io/chaosblade-exec-jvm#164 )


## v1.0.0-GA (Rlease Time:2021.3)
This is a production-ready GA version, fixes some bug.

Features/Enhancements
* Servlet return custom status code(4xx,5xx). (chaosblade-io/chaosblade-exec-jvm#166 )


## v1.2.0 (Rlease Time:2021.5)
This version enhances stability and fixes the problem of slow pod execution for a large number of pods and separate cli, chaosblade-exec-os.

Features/Enhancements
Support async create. (#504 )
Separate cli and exec-os. (#505)
Parallelize exec command in matched pods. (chaosblade-io/chaosblade-operator#78 )


## v1.3.0(Rlease Time:2021.12)
This version adds many new Java plugins, enhances the kubernetes experiment capabilities, and fixes many problems.

Features
* Support download mode for deploying chaosblade tool to target container. (#553)
* Support chaosblade-tool daemonset yaml configuration. (#527)
* Support for using container-name to execute container experiments .(#522)
* Add action and flag parameter in status command.(#519)
* Add chaosblade-override flag to re-deploy chaosblade tool to target container. (#523)
* Add refresh flag to support java agent reloading. (#528)
* Change jvm-sandbox namespace from default to chaosblade. (#525)
* Support systemd stop feature. (chaosblade-io/chaosblade-exec-os#90)
* Support spring cloud gateway plugin. (chaosblade-io/chaosblade-exec-jvm#197)
* Support jvm fullgc experiment. (chaosblade-io/chaosblade-exec-jvm#184)
* Support logback plugin for chaos. (chaosblade-io/chaosblade-exec-jvm#183)
* Support regex pattern parameter for servlet to minimize blast radius. (chaosblade-io/chaosblade-exec-jvm#177)
* Support httpclient timeout feature. (chaosblade-io/chaosblade-exec-jvm#174)
* Support for specifing javaHome when creating java experiments. (#551)


## v1.5.0 (Rlease Time:2022.1)
This version supports Kubernetes v1.22 and fixes some bugs of the previous version. Supports Java experimental scenes in the container.

Features
* Support Kubernetes v1.22. (chaosblade-io/chaosblade-operator#129)
* Support for in-container Java experiments. (chaosblade-io/chaosblade-exec-cri#1)
* Support getBusinessParams method in Dubbo Provider scene (chaosblade-io/chaosblade-exec-jvm#217)


## v1.6.0-alpha Latest (Rlease Time:2022.4)
This release mainly updates execution through the input process namespace, no longer requires the copy tool, this is the alpha release, please use caution.

Features
* Experiment by entering the process namespace, eliminating the need for replication tools
* Merge docker and cri exp
* Support container jvm exp
* Merge OS bin to reduce package size
