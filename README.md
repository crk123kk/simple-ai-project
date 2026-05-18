## 介绍

    这是一个用于给初始创建的项目提供的模板，之后还会有关于旧的项目或者迁移项目中会用到的一些零散模板，会总结出来需要用到的command、skill等

    这一个是无关于技术栈的模板，之后会扩展出关于 vue、next等技术栈相关的模板

## agent 和 IDE 的区别和联系

    理解 agent 和 IDE 之间的区别和联系，cc是有配置的，每个项目也可以配置单独的内容

        agent 是整个电脑上的，使用cc好像最开始打开的地方就是整个系统吗？还是怎么配置的？配置整个系统的是放在哪里？配置给单独的项目又是放在哪里，创建项目的时候会创建到哪里？是哪里打开cc，就在哪里创建吗

## mdc & md

    指令 commands 要用 md 文件格式，而不是 mdc

    Cursor 里 Project Commands（斜杠命令） 只会从 .cursor/commands/ 里读 .md 文件。

    rules 一般用 mdc文件格式

## rule

    如果选择 alwaysApply: true 那么 globs 可以忽略不加，因为加了也没有用

    如果选择 false，就需要对 globs 进行配置，来指定哪些文件需要应用这个 rule

## command、skill、agent

    这三者的区别在于：

        - command 是用户输入斜杠命令时触发的功能，通常用于执行特定的操作或任务。
        - skill 是指系统具备的能力或技能，可以被命令调用来完成特定的功能。
        - agent 是指一个智能体，可以根据用户的输入和环境信息自主地执行任务，通常具有更复杂的行为和决策能力。

    我的理解：

        - command 是入口，是按钮，是用户可以主动触发的事件
            用户主动触发按钮

        - skill 是能力，是功能，是用户可以调用的工具，可以通过指令调用，也可以被 agent 调用
            用户通过主动触发按钮来调用skill，高级的skill也可以做成一个多个步骤的流程，形成一个workflow

        - agent 是智能体，是一个具有自主决策能力的实体，可以根据用户输入和环境信息来执行任务，通常具有更复杂的行为和决策能力。
            用户也可以主动调用agent或者通过按钮来调用agent，然后通过agent来调用skill来完成任务
            并且agent可以理解成一个 workflow，可以包含多个步骤，每个步骤可以调用不同的skill来完成任务

## 一个基本的 ai 系统可以包含

    .cursor/.claude

        - rules（规则层） —— 限定 ai 行文

        - commands（命令层）    —— 主动触发的功能

        - skills（技能层）  —— ai 具备的能力

        - agents（智能体层）    —— 具有自主决策能力的实体

        - workflows（工作流层）    —— 一系列步骤组成的流程，可以包含多个 agent 和 skill


    AGENT.MD/CLAUDE.MD：项目的介绍，让ai了解这个项目的背景、技术栈、架构等信息

    AI_GUIDE.MD/AI_LEARN.MD：ai 避错、学习指南，操作过程中 ai 可能会犯错，这个文档可以帮助 ai 学习如何避免犯错，或者当犯错时如何纠正错误

## 目前阶段的 ai 系统

    commands

        固化了的提示词，并且workflow也是不同提示词的综合，之后可以完善优化整个体系

        比如：
            commit 可以是一个md文件，也可以是一个skill

            command的时候就是简化的skill，但是skill可以更加的完善：包含了：rule、流程、身份等信息
