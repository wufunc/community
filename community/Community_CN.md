# ChaosBlade Community

ChaosBlade是一个开放且活跃的社区，专注于混沌工程学科的探索与实践，非常欢迎每一个有意愿的开发者与我们一起共建开源社区。

这里是开发者指南 - 关于如何提交代码、成员阶梯、相关会议等。如果您想参与到我们的开源社区建设中，阅读此文档是一个很好的开始。

## 社区会议

ChaosBlade社区将于每双周周周五的下午7点举行视频会议（从2022年6月17日开始），来讨论ChaosBlade的现状和发展规划。参与双周会能够让您更快的了解ChaosBlade正在做什么，这将有助于您更好的参与到开源社区来，更方便的提出您的建议以及明确参与贡献的方向。

Regular Community Meeting:

* Thursday 7:00pm Beijing Time (Bi-weekly, Starting 6.17, 2022).
  
Quickly Link:

- [Meeting Calendar](https://calendar.google.com/event?action=TEMPLATE&tmeid=cnM2cGJjYmdmYThvaGVoZjY4M21lZWprdXNfMjAyMjA2MTdUMTEwMDAwWiBjYW1peDAxMTZAbQ&tmsrc=camix0116%40gmail.com&scp=ALL)
- [Meeting Link](https://zoom.us/j/99932900142?pwd=dlFQYWRzdWZaSDVZd1NkUzcydjZFUT09)
- [Meeting Documentation](TODO_会议文档)
- [Meeting Recordings(bilibili)](TODO_会议记录（bilibili）)
- [Meeting Recordings(youtube)](TODO_会议记录（youtube）)

## 贡献者阶梯

我们鼓励每一位感兴趣的开发者都成为社区的贡献者，这通常只需要简单的几步来参与到社区中即可，例如出席会议、报告并偶尔解决问题、或公开宣传本项目.在深入了解本项目后也可承担不同的贡献者角色，我们的项目组成员很乐意帮助您沿着贡献者阶梯前进。在我们的[社区贡献者阶梯文档](./Contributor%20Ladder_CN.md)中了解有关会员要求和责任的更多信息。

在参与贡献前，请阅读[CONTRIBUTING](https://github.com/chaosblade-io/chaosblade/blob/master/CONTRIBUTING.md)

如果您满足成为ChaosBlade成员晋升（Memeber、Reviewer、Maintainer）的要求，可通过[提交issue](TODO_社区ISSUE链接)来申请

## 治理
ChaosBlade按场景领域实现封装成一个个单独的项目，对任何一个项目的贡献都会计入到贡献者阶梯的晋升要求中。
* [chaosblade](https://github.com/chaosblade-io/chaosblade)：混沌实验管理工具，包含创建实验、销毁实验、查询实验、实验环境准备、实验环境撤销等命令，是混沌实验的执行工具，执行方式包含 CLI 和 HTTP 两种。提供完善的命令、实验场景、场景参数说明，操作简洁清晰。
* [chaosblade-spec-go](https://github.com/chaosblade-io/chaosblade-spec-go): 混沌实验模型 Golang 语言定义，便于使用 Golang 语言实现的场景都基于此规范便捷实现。
* [chaosblade-exec-os](https://github.com/chaosblade-io/chaosblade-exec-os): 基础资源实验场景实现。
* [chaosblade-exec-docker](https://github.com/chaosblade-io/chaosblade-exec-docker): Docker 容器实验场景实现，通过调用 Docker API 标准化实现。
* [chaosblade-exec-cri](https://github.com/chaosblade-io/chaosblade-exec-cri): 容器实验场景实现，通过调用 CRI 标准化实现。
* [chaosblade-operator](https://github.com/chaosblade-io/chaosblade-operator): Kubernetes 平台实验场景实现，将混沌实验通过 Kubernetes 标准的 CRD 方式定义，很方便的使用 Kubernetes 资源操作的方式来创建、更新、删除实验场景，包括使用 kubectl、client-go 等方式执行，而且还可以使用上述的 chaosblade cli 工具执行。
* [chaosblade-exec-jvm](https://github.com/chaosblade-io/chaosblade-exec-jvm): Java 应用实验场景实现，使用 Java Agent 技术动态挂载，无需任何接入，零成本使用，而且支持卸载，完全回收 Agent 创建的各种资源。
* [chaosblade-exec-cplus](https://github.com/chaosblade-io/chaosblade-exec-cplus): C++ 应用实验场景实现，使用 GDB 技术实现方法、代码行级别的实验场景注入。

## 路线图
您可通过[路线图](./Roadmap.md)来了解ChaosBlade的发展历程和未来规划
![](./roadmap.png)

## 联系我们

欢迎提交缺陷、问题、建议和新功能，所有项目（包含其他子项目）的问题都可以提交到[Github Issues](https://github.com/chaosblade-io/chaosblade/issues)

你也可以通过以下方式联系我们：
* 钉钉群（推荐）：23177705
* Gitter room: https://gitter.im/chaosblade-io/community
* 邮箱：chaosblade.io.01@gmail.com
* Twitter: chaosblade.io

