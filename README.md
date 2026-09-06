# Agent-RAG-KB-Project
企业研发知识库Agent， Java后端结合RAG大模型
# Java‑RAG‑Agent‑KB‑Project
自研RAG知识库问答Agent，基于SpringBoot后端实现。

## 📖项目简介
本项目为Java后端自研知识库Agent，封装大模型HTTP客户端，实现RAG知识库问答能力。
不依赖现成RAG框架，自己实现分层架构。

## 🧱项目分层结构
- controller：http接口接收层，负责接收请求返回响应
- agentbiz.service：业务服务层，RAG核心业务逻辑（文档切分、知识库检索）
- infrastructure：基础设施层，封装外部依赖（大模型调用客户端、向量库客户端）
- common：通用组件，统一返回体、工具类
- dto：请求响应数据封装

## ✅当前进度（35%）
1. SpringBoot脚手架、Maven依赖、项目分层搭建完成
2. 基础设施：封装大模型HTTP调用客户端，配置读取，异常处理
3. 业务层：实现文档文本切分服务
4. 跑通Mock模拟版RAG问答链路

## 🚧待开发
- 接入向量数据库，实现文档入库、相似度检索
- 文档上传接口
- 完整RAG链路，去除模拟数据
- 片段过滤、prompt优化、边界异常处理

## ⚠️注意
application.properties配置文件不提交仓库，大模型密钥使用本地配置。
