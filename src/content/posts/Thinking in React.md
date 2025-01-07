---
title: Thinking in React
pubDate: 2025-1-7 23:19:23
categories: ['学习']
description: '记录一下在React课程中学到的'
slug: 学习
---

# THE "THINKING IN REACT" PROCESS

1. 将界面分解成一个个的组件，同时思考该如何建立组件树

   - 找出可重用的UI部分
   - 遵循单一职责原则
   - 按照数据模型划分组件

2. 先建立静态版的React界面，不要考虑使用State

   - 自上而下或自下而上构建
   - 使用props传递数据
   - 不要使用state，保持简单

3. 确定最小完整的State表示

   - 确定哪些数据是state
     - 是否通过props传入？
     - 是否随时间保持不变？
     - 是否可以从其他state或props计算得出？
   - 使用何种state：局部state还是全局state
   - 确定state的放置位置
     - 找出使用该state的所有组件
     - 找到它们的共同父组件

4. 确定State的更新方式
   - 确定State更新的方向（单向数据流）
   - 实现状态更新函数
   - 子组件通过回调函数与父组件通信
