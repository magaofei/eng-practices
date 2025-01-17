# 处理代码审查中的回退



有时开发人员会推迟代码审查。他们要么不同意
根据你的建议或他们会抱怨你太严格了
一般。

## 谁是对的？ {#who_is_right}

当开发人员不同意您的建议时，请先花点时间考虑一下
如果他们是正确的。通常，它们比您更接近代码，所以
他们可能真的对它的某些方面有更好的洞察力。他们的
论证有道理吗？从代码健康的角度来看它是否有意义？如果是这样，
让他们知道他们是对的，让问题下降。

但是，开发人员并不总是对的。在这种情况下，审稿人应该
进一步解释为什么他们认为他们的建议是正确的。一个好的
解释说明了对开发人员的回复的理解，以及
有关为何要求更改的其他信息。

特别是，当审稿人认为他们的建议会改进代码时
健康，他们应该继续倡导变革，如果他们相信的话
最终的代码质量改进证明了所要求的额外工作。
**改善代码健康状况往往只需很短的步骤。**

有时需要几轮解释之前的建议
沉入。只要确保始终保持[礼貌](comments.md# courtesy)并让
开发人员知道你*听到*他们在说什么，你只是不同意*。

## 扰乱开发者{#upsetting_developers}

审稿人有时认为，如果审稿人，开发人员会感到不安
坚持改进。有时开发人员会感到不安，但确实如此
通常是短暂的，他们后来非常感谢你帮助他们改进
他们的代码质量。通常，如果你是[礼貌](comments.md# courtesy)in
你的意见，开发人员实际上根本不会感到沮丧，担心的是
只是在评论家的脑海里。沮丧通常更多
[评论的方式](comments.md# 礼貌)而不是审稿人的
坚持代码质量。

## 稍后清理{#later}

推迟的一个常见原因是开发人员(可以理解)想要获得
做的事情。他们不想再进行另一轮审查
这个CL in。所以他们说他们会在以后的CL中清理一些东西，从而你
应该LGTM *这* * CL现在。一些开发人员非常擅长这一点，而且会
立即写一个修复问题的后续CL。然而，经验表明
随着开发人员编写原始CL后经过的时间越长，越少
可能这种清理工作即将发生。事实上，通常除非开发人员这样做
在目前的CL之后立即清理*，它永远不会发生。事实并非如此
因为开发人员不负责任，但因为他们有很多工作要做
在其他工作的压力下，清理工作就会丢失或遗忘。因此，它是
通常最好坚持开发人员现在*之前清理他们的CL *
代码在代码库中并“完成”。让人们“以后清理东西”是一个
代码库退化的常用方法。

如果CL引入了新的复杂性，则必须在提交之前将其清除
除非它是[紧急](../emergencies.md)。如果CL暴露周围
问题，他们现在无法解决，开发人员应该提交一个错误
清理并将其分配给自己，以免它丢失。他们
也可以选择在引用该字段的代码中编写TODO注释
错误。

## 关于严格性的一般投诉{#strictness}

如果您以前有相当宽松的代码审查，并切换到严格
评论，一些开发人员会非常抱怨。改善
代码审查的[速度](speed.md)通常会导致这些投诉消失
远。

有时，这些投诉可能需要数月才能消失，但最终还是会消失
开发人员倾向于看到严格的代码审查的价值，因为他们看到了什么伟大
他们帮助生成的代码。有时最响亮的抗议者甚至成为你的
最强烈的支持者一旦发生事情导致他们真正看到了
通过严格来增加你的价值。

## 解决冲突{#conflicts}

如果您遵循以上所有内容但仍然遇到冲突
你自己和一个无法解决的开发者，请参阅
[准则审查标准](standard.md)指导原则
可以帮助解决冲突。