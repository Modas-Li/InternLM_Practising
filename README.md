# InternLM_Practising
Doing homeworks from InternLM ORG

第一节课：
作业已交飞书文档

第二节课：
基础作业 (结营必做)
使用 InternLM2-Chat-1.8B 模型生成 300 字的小故事（需截图）
实践截图如下：
![img_v3_029j_940f4c74-14e2-4063-9106-8e02b71db36g](https://github.com/Modas-Li/InternLM_Practising/assets/40042370/5b9ab11f-0235-45a6-94ce-f8795421e176)

第三节课：
学习笔记一：
第三节课主要介绍了安装和运行"MMPose"的步骤，以及一个名为"HuixiangDou"的基于LLM（大型语言模型）的知识助手的使用。首先，安装MMPose需要设置Miniconda环境，并创建一个名为openmmlab的conda环境。对于HuixiangDou，需要确保LLM服务正常运行，通过执行python3 -m huixiangdou.service.llm_server_hybrid来检查。在遇到问题时，如500错误，需检查服务端口和配置，以及TOKEN的正确性。若使用docker，LLM服务需要单独部署。
HuixiangDou可以与飞书或个人微信集成，发送技术助手的回复。高级功能包括使用更精确的本地LLM模型、Hybrid LLM Service和repo搜索增强。调优可通过调整配置文件如config.ini进行，包括拒绝和处理问题的策略。此外，提供了Web版的源码，支持多种即时通讯软件，并有硬件需求指南，包括不同版本对GPU显存的需求。对于显存有限的用户，可以使用替代方案。最后，文章提供了错误处理和常见问题的解答，帮助用户更好地理解和部署系统。
![image](https://github.com/Modas-Li/InternLM_Practising/assets/40042370/b7a3c576-01ab-431d-a2bd-79a9b55e6246)
![image](https://github.com/Modas-Li/InternLM_Practising/assets/40042370/3d206cf8-699a-40a3-b1ca-4db5575f91be)

学习笔记二：
"茴香豆"，一个基于RAG技术的知识助手，用于群聊环境。项目结构清晰，包含配置文件、教学文档、代码库和测试部分。核心代码位于huixiangdou/service/worker.py，其中的Prompt可定制，适应不同业务需求。配置文件如config.ini用于设定运行参数。
工作流程涉及Prompt模板，如主题检测、相关性评分、关键词提取、内容安全评估和复杂度评分等。此外，还支持网络搜索功能，通过Serper API获取在线信息。用户可配置config.ini启用远程模型，如GPT-4，降低GPU需求。
部署包括创建知识库向量数据库和运行助手。运行时，助手对问题进行相似性比较，检索相关信息生成答案。进阶功能包括网络搜索集成和使用远程大模型。
总结起来，茴香豆是一个可定制的、利用RAG技术的知识检索和生成系统，适用于群聊环境的智能助手，支持本地和云端模型，可扩展网络搜索，提供准确和丰富的解答。
![image](https://github.com/Modas-Li/InternLM_Practising/assets/40042370/de7e6c29-a7b8-46a0-97de-256520e8532b)

第四节课：
训练自己的小助手认知（记录复现过程并截图）
训练过程截图：
![image](https://github.com/Modas-Li/InternLM_Practising/assets/40042370/ded85b13-23d6-4f28-bb1f-f5a22128e0e9)
模型对话截图：
![image](https://github.com/Modas-Li/InternLM_Practising/assets/40042370/dd9a9dc1-1a56-4409-be47-083bc0e33640)
![image](https://github.com/Modas-Li/InternLM_Practising/assets/40042370/5c003160-7a74-4b4a-a2c5-5383a8f28424)
web demo:
![image](https://github.com/Modas-Li/InternLM_Practising/assets/40042370/f17bc94e-bfc8-441f-a3d2-c5ea6a1cd64b)
