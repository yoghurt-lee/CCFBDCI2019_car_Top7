# CCFBDCI2019_car_Top7
CCFBDCI 2019乘用车销量预测复赛B榜(7/2999)

我们是CCFBDCI 2019乘用车细分市场销量预测的队伍，麓南小聪明。
我们队伍初赛A榜14名，B榜第34名。复赛A榜14名，B榜第七名(0.61991131)。

我们采用了模型和规则两种方案.
其中模型我们最终的分数是0.592 ，规则是0.587 ，采用 6: 4进行融合 (这里有点失误，我最终交的文件是用的0.589的模型融合的，所以说最终的结果应该是比6199要高的 = =)。

- lgb_new.ipynb 和 lgb_old_1.ipynb 分别是对新车型和旧车型进行预测的文件，这里的话是采用鱼佬的框架，然后加上了几个特征。

- rule_587.ipynb 是我们所用的规则 这里的用根号平滑了趋势 然后用指数平滑来对销量进行了修正。
