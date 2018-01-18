# KSQL 手册

| 概览 |[入门](/docs/quickstart#quick-start) | [概念](/docs/concepts.md#concepts) | [语法](/docs/syntax-reference.md#syntax-reference) |[演示](/ksql-clickstream-demo#clickstream-analysis) | [样例](/docs/examples.md#examples) | [FAQ](/docs/faq.md#frequently-asked-questions) |
|---|----|-----|----|----|----|----|

> *重要：当前版本仍处于 **开发者预览** 状态，由 Confluent 支持并且免费，开源，基于 Apache License 2.0。请勿在任何生产集群运行 KSQL。*

# 概览
KSQL是一个开源的流式 SQL 引擎，针对 Apache Kafka 实现了连续性，交互式的查询功能。只需要通过 SQL 命令即可对 Apache Kafka 中的数据进行实时的查询，读取，写入，和处理。KSQL 直接与 [Kafka Streams API](https://kafka.apache.org/documentation/streams/) 交互，因此建立一个 Java 应用不再对其有依赖。

### 应用场景
通常 KSQL 有下列应用场景：

- 欺诈识别 - 识别和处理超出正常范围的数据，实时感知。
- 个性化 - 根据数据为终端用户创建实时体验和用户画像。
- 通知 - 基于实时数据创建自定义的告警和消息。
- 实时分析 - 强大的实时仪表盘以了解当前正在发生的事件。
- 传感器数和物联网 - 随时随地的获取和传输传感器数据。
- 客户 360 度描述 - 针对客户各个方面提供更清晰和实时的理解。

KSQL 降低了在你的应用中使用实时数据的门槛。它建立在一个可扩展的流式平台之上，不像其他流式处理方案那样需要额外的学习成本或者复杂的管理。

## 应用模式
KSQL 的应用模式包含 独立模式，客户端-服务器模式，应用模式，和嵌入式模式。更多细节，请参考 [概念](/docs/concepts.md#concepts)。

## 开始使用

* 初学者：参考 [交互式入门](/docs/quickstart#quick-start)。该入门配置了一个在轻量级 Docker 或者 Kafka 集群中运行的 KSQL 实例。并演示了一个通过 KSQL 来编写流式查询语句并查询 Kafka 中数据的简单工作流程。
* 进阶用户：参考 [端到端点击流分析演示](/ksql-clickstream-demo#clickstream-analysis)。

## 兼容性

下表给出了 KSQL 的读写查询所能支持的 Kafka 版本兼容性矩阵。

|        KSQL        |        0.1       |        0.2       |        0.3       |
|:------------------:|:----------------:|:----------------:|:----------------:|
|    Apache Kafka    |      0.10.1 +    |      0.10.1 +    |     0.10.1 +     |
| Confluent Platform |      3.1.0 +     |      3.1.0 +     |     3.1.0 +      |
