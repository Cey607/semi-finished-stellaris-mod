<style>
    .hover-text {
        position: relative;
        display: inline-block;
    }
    .hover-text::before {
        content: '';
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        background-color: black;
        z-index: 1;
    }
    .hover-text:hover::before {
        display: none;
    }
     .hover-image {
        position: relative;
        display: inline-block;
    }
    .hover-image img {
        display: block;
        width: 300px; 
        height: auto;
    }
    .hover-image::before {
        content: '';
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        background-color: black;
        opacity: 1; 
        z-index: 1;
        transition: opacity 1s;
    }
    .hover-image:hover::before {
        opacity: 0;
    }
</style>
# 一个瞎鸡掰做的mod
## 这是一个***仍在开发中***的群星的模组:

1. 这玩意我也不知道会鸽多久<sub>~~自己做游戏去咯~~</sub>
2. 包含了一个轨道轰炸
3. 包含了一个开局的小助手(类似一个提供buff的小灰)
4. 魔怔数值怪武器和global_ship_design
5. 包含一个星球类型和它的附属区划
6. 替换了**所有**国家的恒星基地模型为堕落帝国的
7. 包括了一个我*试图*扩展为天灾的事件(关于蠢驴country_type的ai模块到现在我也没摸清楚)
8. 包括两个封装好的脚本，一个是清理全银河除玩家之外的default国家，另一个是在全银河范围内生成pre_ftl土著并将其中一部分提升为普通国家<sub>打不过就重开</sub>但是这两个脚本没有任何调用，只能通过控制台输入
9. 其中轨道轰炸的部分已经上线[steam创意工坊](https://steamcommunity.com/sharedfiles/filedetails/?id=3207454994)

### 目前已知bug很多
- 中期之后出现的天灾舰队水平计算的逻辑不太可靠,可能对一部分电脑国家造成很严重的影响
- 轨道轰炸会在星球上生成陆军,在占领之后解散陆军,**但是**如果一个星球被攻占时另一个星球有这个轰炸姿态创建的陆军正在作战,它们会被一起清除.(我知道不应该在国家域里操作,但是星球域操作我不知道陆军打完什么时候上船,总是清理不掉)
- 缺少大量文本和UI
- 没有主线,想到哪做到哪,纯纯乐子mod
- 天灾的舰队实力是动态的,也就是说这玩意在后期可能对渣机和用了魔怔mod的电脑造成物理伤害,我临时添加了限制和新的舰队构成比例,应该能缓解一点<div class="hover-image">就一点点</div>
