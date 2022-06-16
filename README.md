# ChaosBlade Community
[中文社区文档](Community_CN.md)

ChaosBlade is an open and active community that focuses on the exploration and practice of chaos engineering disciplines. Every willing developer is very welcome to build an open source community with us.

Here's the developer guide - on how to commit code, member ladders, related meetings, and more

## Community meeting

The ChaosBlade community will hold video conferences every biweekly Friday 7:00pm (starting from 17th June, 2022) to discuss the current status and development plans of ChaosBlade. Participating in the bi-weekly meeting will allow you to understand what ChaosBlade is doing more quickly, which will help you better participate in the open source community, make your suggestions more easily, and clarify the direction of participation and contribution.

Regular Community Meeting:

* Friday 7:00pm Beijing Time (Bi-weekly, Starting 17th June, 2022).
  
Quickly Link:

- [Meeting Calendar](https://calendar.google.com/event?action=TEMPLATE&tmeid=cnM2cGJjYmdmYThvaGVoZjY4M21lZWprdXNfMjAyMjA2MTdUMTEwMDAwWiBjYW1peDAxMTZAbQ&tmsrc=camix0116%40gmail.com&scp=ALL)
- [Meeting Link](https://zoom.us/j/99932900142?pwd=dlFQYWRzdWZaSDVZd1NkUzcydjZFUT09)
- [Meeting Documentation](TODO_会议文档)
- [Meeting Recordings(bilibili)](TODO_会议记录（bilibili）)
- [Meeting Recordings(youtube)](TODO_会议记录（youtube）)

## Contributor ladder

We encourage every interested developer to become a contributor to the community, which usually only takes a few simple steps to participate in the community, such as attending meetings, reporting and occasionally solving problems, or publicly promoting the project. There are also different contributor roles available with an in-depth understanding of the project, and our project team members are happy to help you along the contributor ladder. Learn more about membership requirements and responsibilities in our [Community Contributor Ladder Document](Contributor_Ladder.md).

Please read [CONTRIBUTING](https://github.com/chaosblade-io/chaosblade/blob/master/CONTRIBUTING.md) before contributing

If you meet the requirements to become a ChaosBlade member for promotion (Memeber, Reviewer, Maintainer), you can apply through [Submit an issue](TODO_社区项目ISSUE链接)


## Governance
ChaosBlade is encapsulatd into separate projects according to the scene field, and contributions to any project will be included in the promotion requirements of the contributor ladder.
* [chaosblade](https://github.com/chaosblade-io/chaosblade): Chaos experiment management tool, including commands for creating experiments, destroying experiments, querying experiments, preparing experimental environments, and canceling experimental environments. It is the execution of chaotic experiments. Tools, execution methods include CLI and HTTP. Provides complete commands, experimental scenarios, and scenario parameter descriptions, and the operation is simple and clear.
* [chaosblade-spec-go](https://github.com/chaosblade-io/chaosblade-spec-go): Chaos experimental model Golang language definition, scenes implemented using Golang language are easy to implement based on this specification.
* [chaosblade-exec-os](https://github.com/chaosblade-io/chaosblade-exec-os): Implementation of basic resource experimental scenarios.
* [chaosblade-exec-docker](https://github.com/chaosblade-io/chaosblade-exec-docker): Docker container experimental scenario implementation, standardized by calling the Docker API.
* [chaosblade-exec-cri](https://github.com/chaosblade-io/chaosblade-exec-cri): Container experimental scenario implementation, standardized by calling the CRI.
* [chaosblade-operator](https://github.com/chaosblade-io/chaosblade-operator): Kubernetes platform experimental scenario is implemented, chaos experiments are defined by Kubernetes standard CRD method, it is very convenient to use Kubernetes resource operation method To create, update, and delete experimental scenarios, including using kubectl, client-go, etc., and also using the chaosblade cli tool described above.
* [chaosblade-exec-jvm](https://github.com/chaosblade-io/chaosblade-exec-jvm): Java application experimental scenario implementation, using Java Agent technology to mount dynamically, without any access, zero-cost use It also supports uninstallation and completely recycles various resources created by the Agent.
* [chaosblade-exec-cplus](https://github.com/chaosblade-io/chaosblade-exec-cplus): C ++ application experimental scenario implementation, using GDB technology to implement method and code line level experimental scenario injection.

## Road map
You can learn about ChaosBlade's development history and future plans through the [roadmap](./Roadmap.md)
![](./roadmap.png)


## Contact us

For bug report, questions and discussions please submit [GitHub Issues](https://github.com/chaosblade-io/chaosblade/issues).

You can also contact us via:
* Dingding group (recommended for chinese): 23177705
* Slack group: [chaosblade-io](https://join.slack.com/t/chaosblade-io/shared_invite/zt-f0d3r3f4-TDK13Wr3QRUrAhems28p1w)
* Gitter room: [chaosblade community](https://gitter.im/chaosblade-io/community)
* Email: chaosblade.io.01@gmail.com
* Twitter: [chaosblade.io](https://twitter.com/ChaosbladeI)

