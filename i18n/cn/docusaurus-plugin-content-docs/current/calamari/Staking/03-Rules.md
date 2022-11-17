# 规则

一个 Calamari 网络参与者的角色可以是：

- 委托者
- Collator
- 不参与 Staking 质押

每个角色适用不同规则，Collator 和委托者的角色只能选择其一。如果需要转换角色，则需要先解绑 KMA，再重新绑定成为另一个角色。

## 对于委托者（Delegators）

- 最低质押数量：5000 枚KMA
- 每个 Collator 能接收的最大委托者数量：100个

    - 若 Collator 拥有超 100个委托者， 获得奖励所需 KMA 最低质押数量将大于 5000 枚，具体取决于其他委托者的质押数量。可查询委托 dApp，查看当前最低质押数额要求

- 取消委托或减少委托金额，需要 7天等待期
- 你质押的 KMA 在该 Collator 中占比越高，获得的奖励就越多
- 若选择的 Collator 未排在前 63 位，你将不会获得奖励
- 若你委托的 KMA 数量，在该 Collator 委托数额中，未排进前 100，则不会获得奖励
- 你可以将 KMA 分散质押给一个或多个 Collator
- 奖励周期时长6小时，这称为轮次
- 奖励会在 2轮后，自动发送到委托者地址上
- 奖励无自动复投， 最多可选择分配给 25个 Collator
- 目前尚没有惩罚机制。

## 对于 Collator

- 成为 Collator候选者，需至少质押 400万枚 KMA
- 可获得奖励的最大 Collator 活跃数量：63
- Collator 排名由其上质押的 KMA 总量决定（包括 Collator 和所有委托人质押的 KMA 总和）
- 单个 Collator 上最大活跃委托者数量（可计算排名的质押 KMA 总量）：100
- 奖励周期时长6小时，这称为轮次
- 奖励会在 2轮后，自动发送到 Collator 地址上
- 奖励无自动复投
- 取消或减少保证金，需要 7天等待期
- 无法将保证金减少到 400万枚 KMA 以下（除非移除 Collator 角色）
- 若错过区块，目前没有惩罚机制，但你的委托者们不会喜欢错过奖励