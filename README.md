# CCFBDCI 2019乘用车销量预测复赛B榜(7/2999) 方案分享

赛提地址: https://www.datafountain.cn/competitions/352
我们是CCFBDCI 2019乘用车细分市场销量预测的队伍，麓南小聪明。

我们队伍初赛A榜14名，B榜第34名。复赛A榜14名，B榜第七名(0.61991131)。

我们采用了模型和规则两种方案.
其中模型我们最终的分数是0.592 ，规则是0.587 ，采用 6: 4进行融合 (这里有点失误，我最终交的文件是用的0.589的模型融合的，所以说最终的结果应该是比6199要高的 = =)。

- lgb_new.ipynb 和 lgb_old_1.ipynb 分别是对新车型和旧车型进行预测的文件，这里的话是采用鱼佬的框架，然后加上了几个省份(adcode)，车型(adcode)的趋势特征。

- rule_587.ipynb 是我们所用的规则 按照上半年和下半年统计了省份(adcode)，车型(adcode)趋势特征 这里的用根号平滑了趋势 然后用指数平滑来对销量进行了修正。

- mix_lgb592_rule_587(B-6199).ipynb 是我们用来进行融合的文件，融合很简单，就是按照6比4直接进行融合。

这个比赛我们打得比较佛系，没想到最后到了前排，希望大佬们也能够开源，让我们学习一下~
