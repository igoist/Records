## Log of my daily life 讲生活，谈心情 2020 年 1 月 2 日至 X 月 X 日


备忘：

inquirer (/live/node_modules/inquirer)

* message 组件多版本重现

好家伙！新京报、澎湃新闻、财新杂志、财经杂志、北京青年报、三联、中国新闻周刊、第一财经、21世纪经济报道、界面新闻

石油风云

屏蔽 hotbak.net

岗山步兵百十联队史


### 2020.02.18

不好意思青青阿舅，跟工作挤一块了，我只能大概地写了写，感觉也帮不上你什么忙：

1. 因为我没有做过人才招聘这块领域的开发，开发过程中会有哪些比较关键、不应该被糊弄过去的技术结点，我一下子实在是没法预见、回答，建议只能是再根据方案表，和现成的其他政府机构的人才网、招聘网站，boss直聘、拉勾网、智联招聘、前程无忧、58、赶集这些平台都一一对照看看，有哪里是需要改进的、补充的，哪里是被遗漏的。

2. 不管微信小程序还是 PC 端，都应该是去调用部署在服务器上的后端的接口，而不是什么直接读数据库。租用服务器，就要根据 3 的服务器实际参数容量考虑性价比来做出选择，至于是阿里云还是腾讯云关系不大。

3. 最开始的开发测试阶段，不论阿里云还是腾讯云的最低配的服务器，都足够用来部署这个网站的前后端，等后面正式上线运营之前才需要提前根据预计的访问量相关等在服务器供应商这边做好扩容，再后面要根据运营期间实际访问量、发布人力资源信息后数据库内存储量的增加等实际情况来动态扩容，至于具体的参数，在我公司里，应该是问后端、运维的人员，我毕竟是前端，对此不了解。

4. 这个完全是要看整个网站前后端开发得怎样、后期甲方这边会不会频繁提出新的需求。如果开发得好、后面甲方这边新的需求不多，主要工作内容真的只是发布一些广告信息、偶尔调整网站的页面，那么这个岗位的技术人员，平常工作量就不大，只需要具有掌握比较基础的前后端和运维知识即可胜任；但一般情况下，交接后还是会有这样那样的新需求提出来，前后端都会需要在前面人写的代码的基础上进行二次开发，对相关知识掌握情况的要求就进一步提高。打比方项目交接后王二应聘了这个岗位，后面他离了职又来了张三李四，如果他们技术都比较好，再后面可以有王五赵六来接替，可要是王二、张三都技术奇差滥竽充数，每次新的需求写乱七八糟，往项目里胡乱添加代码，很可能等他们离职后李四王五赵六看看项目代码，里面浆糊一样一团乱麻，便一个个都不敢来接手，要么这个项目到此为止，要么再花费非常高的价格请一个厉害的人来大刀阔斧地重构。我把我知道的情况都例举出来了。

fd5259ae4

### 2020.02.14

我来给这个题目再转译一下吧：

张三问王二：“王二！你看俺才初一就晓得了怎么使用石器、榔头、石斧、锤子、锯子、斧头，俺是不是完全超越了同龄人、特别牛（理直气壮，作叉腰状）？！”

王二答：“阿三哥真厉害！小弟当年还在捏尿泥、掏鸟蛋，比不上您一毫，那会别说榔头、石斧、锤子、锯子、斧头，就连石器也从没听过。”

说真的，按照楼主的标准来算，王二身边做技术的同事们人人都会十种以上编程语言（但日常工作中真正在使用的，无非是针对项目特定几种）。

仅仅学会/掌握一种语言/工具/手段，很多时候真的只是不值一提的长处。

但如果说张三哪天通过这些不起眼的工具，不单只会造茅屋，还能从无到有，建造起了什么香榭亭台、楼阁宫阙，又或者通过改进榔头，设计出榔头 普拉斯（不一定非得自己亲自实现/制造），榔头普拉斯麦克斯，甚至将各种石器、榔头、石斧、锤子、锯子、斧头融合超进化，设计出什么盾构机、千吨级架桥一体机诸如此类更高阶的工具，那时的张三将早已充满自信，不会再考虑什么作为个体超越不超越这种无聊的问题。


### 2020.02.11

“与之交谈，两目瞪然视，舌木强不能对”

お金なんかじゃ　　人の心は　買えやしないわよ

### 2020.02.09

错误的处理方式：以如此“积 极”的态度跑班级群里没羞没臊地诡辩、强词夺理，任由罪魁祸首当事人在家若无其事、悠哉悠哉避（打）风（游）头（戏）

正确的处理方式：把小兔崽子一路从校门拎到讲台上，当着大家的面，pia！一个大耳光！pia！又一个！pia！三个四个五个六个七个八个...  直到“哎呀.. 阿姨/叔叔别打了！...” “XXX妈妈/爸爸别打了！...” 最后再让他好好给女生、给所有人道个歉，反省反省为什么要道歉

（但对于这种人，我真实想法是，毁灭吧，赶紧的）


### 2020.01.29

<blockquote>

公司主站这项目说得好听点叫百废待兴

说得难听点就是以前几乎等于啥都没有，断层异常严重，这人这里这样写一点，那人那里那样写一点，终于变成一团乱麻、稀烂、一塌糊涂、一大个烂摊子

为什么我要这么说？因为在收拾烂摊子的那头蠢驴是我！
</blockquote>


### 2020.01.28

<blockquote>

1、History is the triumph of the heartless over the mindless.

2、Four-stage strategy:

stage 1 we say nothing is going to happen;

stage 2 we say something may happen, but we should do nothing;

stage 3 we say maybe we should do something, but there is nothing we can do;

stage 4 we say maybe there was something could have done, but now it's too late.
</blockquote>


### 2020.01.24

<blockquote>

这不是很简单吗？

一旦衣食住行无忧，吃饱喝足有闲了，

无非就是你喜欢做、想做什么事，想成为一个什么样的人，想和什么样的人在一起，想爱什么样的人，在世俗之外至少留有一片自己的天地(精神家园)，

然后怎样动脑筋、努力去实现，

怎样在你之后人生的各个阶段回首往事，能够少一些遗憾
</blockquote>

### 2020.01.13

<blockquote>

拜托，一个普通打工人也就百来斤，顶多算他两百斤。可一头成年的猪或牛呢？几百斤！吃的量就不在一个数量级！按平均算每头每月八百的预算，每天也就二三十。换句话说，每天二三十买的2斤的饭菜，或每天20斤的饲料，你们选哪个？
</blockquote>


### 2020.01.05

<blockquote>

马萨诸塞州一个鞋厂的监工说：“让一个身强力壮体格健全的18岁小伙子，在这里的任何一架机器旁边工作，我能够使他在22岁时头发变成灰白。”
</blockquote>


### 2020.12.30

<blockquote>

需要反馈的内容：

1. 文字需要字体宽度 1.5 倍的行高，（举例：FloraZeng）

2. 中轴 1200px...
</blockquote>


### 2020.12.25

<blockquote>

要我说最有价值的还是索拉卡的大招，全球所有人增加寿命，好家伙:

什么是地球乌托邦啊？

什么是人类命运共同体啊？

（战术后仰）
</blockquote>


### 2020.12.24

<blockquote>

2006年5月，庄羽诉郭敬明案在持续近三年后得到终审判决，认定郭敬明所著《梦里花落知多少》对庄羽的《圈里圈外》整体上构成抄袭，判决郭敬明与春风文艺出版社赔偿庄羽经济损失和精神损失费21万元，并停止相关图书的出版、销售行为。

但郭敬明一直拒不道歉，他在博客上公开回应称，官司打了三年，期间他写了长篇小说、出版了多本图书，唯独没有在官司上浪费精力。他声称，“我会执行法院判决的赔偿和停止销售，那是出于我对法律的尊重。但我不会道歉！金钱、名声，这些东西，真不是那么重要，我都可以给予，惟独道歉，哪怕只是简简单单一句话，也决不会迫于压力而放弃了自己的原则，放弃了曾经创作时的辛苦，放弃了所有依然喜欢着我的文字的人的希望。”

后来，郭敬明被法院强制执行道歉，由法院代拟道歉信刊登在报纸上。官司结束后，一些书店仍在售卖侵权作品《梦里花落知多少》，当时庄羽苦恼地对媒体说，“这个官司纠扯不清，弄得我疲惫不堪，本来我想他道歉完后整个事情就过去了，但没想到还是没完没了。”

于正一直被质疑有抄袭嫌疑，在接受媒体采访时，他曾公开回应：“首先艺术就是继承和发展的，中国电视剧发展那么多年了，你敢说哪一个桥段没被人用过的？还有比如说郭敬明，你说他抄袭，人家告他，他输了，对吧？什么时候有人告于正抄袭了，从来没有吧？”

曾与于正合作过的编剧李亚玲也在此次联名信上签名，她早在微博上公开披露过于正的抄袭手法：“早在2009合作《大丫鬟》时,于正就要求我把《胭脂雪》副线和《梅花烙》主线结合起来写成一部戏给他制作，被我拒绝……还说抄袭只要不超过20%，比如你把20集戏全抄了，但只要扩充到100集法院就不会追究。”
</blockquote>


### 2020.12.23

<blockquote>

中国青年报引用了木心的说法：“万丈深渊，下去，也是鹏程万里。”

木心没说的是，有些人是躲在深渊下面的老狐狸，白天给羊群讲这个道理，晚上就去吃自己掉下去的傻羊。
</blockquote>


### 2020.12.17

<blockquote>

王二修了快一月水管，又觉得重复枯燥且没劲了，便去托之前派出所里的那个大学生小刘帮自己包装投简历。

王二语重心长地嘱咐小刘，一定要帮自己找个有意思点的工作，比方可以开着挖掘机炒菜、边玩边挣钱，或者全世界到处跑之类的。

王二怎么说也是从自己所里出去的、参与过包括“迅雷-2020”多项行动的退休卧底老同志了，小刘不敢怠慢，认认真真...

“挖掘机炒菜，呃，马戏团？边玩边挣钱，网管？...”小刘心想。

那天王二的老爷机诺基亚响铃了，接起来一听，对方介绍说是某...

（王二心想这不是忽悠人、骗子嘛，便打了老领导电话，让他派经侦部门的来查一查，最后一股脑儿捣鼓掉了这家公司？）
</blockquote>


### 2020.12.16

<blockquote>

那天王二刚出桥洞，不快不慢地走着，对面桥洞的老弟追上了王二，说道：“王二你怎么走那么快！是不是急着去工地搬砖？！”

王二一个纳闷，走得更慢了，想着自己走得并不快啊，结果回过神，唉？这兄弟怎么已经走出五十步远？！

于是王二更纳闷了

...

有些事情局外人看不明白，局内的人才懂各种酸甜苦辣，

当然也有不少事情当局者迷旁观者清，

比如说看到人家回答里举了个例子：

“十个孩子九个缺钙！真的吗？”

要是随便一个营销号取了个这样的标题，然后再在文章里面瞎编胡说八道一通，

被个当父亲当母亲的看到了，且生物化学医学科学常识不足，可能就容易，哦呦，好焦虑！

挺逗的
</blockquote>


### 2020.12.11

<blockquote>
那时候一个女生家里比较穷，但长得还不错，便被同学校一个混混缠上了，后来纠缠中被教导主任发现，便把两人都训了一顿。

但是女生耿直，宁死不承认错误，相反男生却知道这种事就坡下驴就好，结果女生被请家长。

女生父亲来了，他父亲是很憨厚的人，大家都知道主任要欺负父亲憨厚，但是万万没想到这个大叔也耿直，死活不认为是女生的错。

教导主任便说出了一句我听了无数遍的话：

一个巴掌拍不响。

他为什么不找别人？

据回来说当时情景的班主任回忆，女生的父亲想反驳这句话，但嘴巴笨，支支吾吾说不出来，教导主任露出了满意的微笑，突然女生的父亲仿佛下了一个艰难的决定。

他打了那个混混一个耳光，不知哪里来的勇气问：

你说，响不响？

那个男生当时就蒙了，大家都蒙了，之后再也没人敢欺负这个女生了。

...

你遇到这件事应该怎么做？

你既不想打人，却又咽不下这口气。

那你就纵容他，夸奖他。

社会会替你教育他。

...

所以当时应该这么说：

老师：喂，家长 B？你的孩子玩具被人抢，还被掐脖子，哮喘病发差一点没命了！

家长B：什么？！谁干的？！我弄死他！.. 等等，我孩子有哮喘？！

老师：哦，不好意思我搞错了，是你家孩子在抢人家玩具，还掐人脖子，搞得人家孩子哮喘病发差一点没命！
</blockquote>



### 2020.11.28

<blockquote>

以后的日子很忙碌了，我该回归之前和尚那样的生活，每天除了吃喝写代码就是学习，AFK 指不定哪天就弃坑了，前面荒废蹉跎拉下的东西都要一点一点补起来。

也就是说，咱们今后几乎没有交集了，而且你也见到了，秃顶，柴油桶一样的身材，身高不足一米六，所以，忘了我吧，过去一年多感谢有你和群友们的陪伴，也祝你今后幸福快乐。
</blockquote>




### 2020.11.22

<blockquote>

你知道我对游戏的看法吗？从 2018 年末陷进 DNF 起，我总是会想自己是在虚度、荒废、蹉跎岁月，常常会想所谓奶头乐

我本以为遇见你，是缘分，算是在虚度的岁月中有所收获

直到真正见到你，我没法骗自己，我没法再继续喜欢你

过去一年多，感谢有你还有其他群友们的陪伴，但是我不好，想不出更好的方式好聚好散，很对不起
</blockquote>


### 2020.11.20

<blockquote>

需要一位厨房能替我打下手，学外语可以陪练，平常一起宅、周末想玩一起出去玩的女同志。急！很急！

...

上学时很鄙视相亲，觉得这是自我侮辱。工作以后，一直在自我侮辱。

...

其实我一直很排斥相亲的。

两个不认识的人突然凑到一起，还都带有目的性的凑一起，一想就能尴尬到脚趾头。

从我现在的结果来看，真香会迟到，但从来不会缺席。（啪啪啪，脸疼）
</blockquote>


### 2020.11.19

<blockquote>

其实完全是一码归一码。

挨再多的毒打，如果人很呆滞或者麻木，不善于自己事后去回顾这种种所经历了的，不去思考各种事情的对与不对、该与不该，不去想有哪些其实可以避免的、摆脱的甚至克服掉的，没有痛定思痛，那么对于个人提高思想深度而言真的没有任何帮助。

就比如王二这个人，至今没挨过什么所谓的社会毒打，

但这不妨碍当他看到听到种种别人嫖娼、包小三搞外遇的事情后，内心很确信自己将来只要不被人下药或者强制威胁，绝对不会在婚内出轨，

...

一个人要是到老了还天真烂漫跟个小孩似的，那你说他这辈子过得得多开心呐。
</blockquote>


### 2020.11.18

<blockquote>

你应该啪的一下站起来，直接告诉他：年轻人，你搞偷袭，不讲武徳。编码的人不能窝里斗，你要耗子喂汁
</blockquote>


### 2020.11.16

<blockquote>

她本可以像我那样过安稳的生活。大学毕业后，她在省城工作了2年，2011年24岁时，她考了老家县城的村官，并被分配到她家附近的小镇。她住在家里，每天早晨搭公交车去镇政府，下午返回，每趟不到半小时，生活被母亲照顾得很好。但仅仅过了两个月，她果断地选择了辞职，因为她感受到了与陆平原同样的痛苦，“我感觉自己瞬间从文明世界掉进蛮荒世界，不可能在那种丛林法则里生存”。

王悦歆是个行动派，所以，听到陆平原的事儿，立马说：“如果你确实感受到强烈的痛苦，那就立刻去解决你的痛苦。你和陆平原之所以同样如此矛盾和痛苦，就是因为你们总是瞻前顾后，既想要这个，又想要那个，而人生不可能两全其美。作为成年人，你只需清楚自己所作选择的后果和代价，对此负责即可，没必要想太多，更不要被未知吓倒，因为人生有无数种可能。”
</blockquote>


### 2020.11.12

<blockquote>

所以总结下来我认为就是两点：1.尽管你手中握着事情的一半，但你永远逃脱不了命运的安排的另一半！2.永远不要放弃希望！

...

下面这一段是，我没有一点点的印象了，全是我老婆记下的：

在我睡着后，过了差不多25分钟，我老婆，喊我，我根本没有一点的反应和回应！

于是她，就用力的推晃我，这时我才有了反应，闭着眼说，到点了啊，问吧，她说，你还清醒吗？你刚才睡着了没？

我没有说话，她推了推我，我才说话，问，你刚才说什么了？

她就又说了一边，我还是闭着眼，说，睡着了，不过真的是不清醒了，有点意识模糊了，还有什么要问的吗？

她说，你知道你今天喝这么多酒是为了什么吗？我说，是为了验证一句话。

她又说，你藏私房钱了吗？我听完后，闭着眼呵呵笑了两声，说，放心吧，没有，我现在还是有思考能力的，就算是有我也会说没有，

只是觉得现在没有力气说话了，行了，快睡吧，明天再说。
</blockquote>

find ~/Library/Application\ Support/Developer/Shared/Xcode/Plug-ins -name Info.plist -maxdepth 3 | xargs -I{} defaults write {} DVTPlugInCompatibilityUUIDs -array-add `defaults read /Applications/Xcode.app/Contents/Info.plist DVTPlugInCompatibilityUUID`
### 2020.11.10

<blockquote>

什么时候我国也发展一些类似“反霸凌机车帮”的组织机构

说真的，将这样的组织推广起来，然后尽可能地通过法制教育、威慑去控制、教化那些刺头，一点点遏制掉直接的霸凌，再通过其他方式减少冷暴力

孩子们的心灵保护好了，孩子间的关系融洽了，未来进入社会，便会少一些傲慢、冷漠
</blockquote>


### 2020.11.09

<blockquote>

上回见这位老兄，还是在中央公园，甚至跟老头子我一起转过陀螺呢，如今居然上了电视，当选了总统，真想不到
</blockquote>


### 2020.11.03

<blockquote>

Imagine life as a game in which you are juggling some five balls in the air. You name them — work, family, health, friends and spirit and you’re keeping all of these in the air.

You will soon understand that work is a rubber ball.

If you drop it, it will bounce back. But the other four balls — family, health, friends, and spirit — are made of glass. If you drop one of these, they will be irrevocably scuffed, marked, nicked, damaged, or even shattered. They will never be the same. You must understand that and strive for balance in your life.
</blockquote>


### 2020.10.31

<blockquote>

坏事做尽但却流芳百世，一生行善但却最终身败名裂
</blockquote>


### 2020.10.30

<blockquote>

看了那个成都纵火案，那种男的就是他妈的人渣混蛋孬种！跳楼真的是便宜了他，害了人胥小敏好好的一个人，连带女儿。

看过不少相似的，真是服了
</blockquote>


### 2020.10.29

<blockquote>

看了篇《一个烂尾小区的催化史》，惊叹于一个吃回扣、瞎搞的吊人的破坏力。肥了他一个，损害了一大圈

...

疫情当前，卫生部长溜溜球了，和刚要开战的时候将军退役异曲同工啊。

...

在面临个人得失和保护社会契约这两者的选择时，理性人都会先考虑个人得失，但最终社会会因为每个人的理性选择而走向更差的处境。

...

怎么看？

和当年国军“歼敌一亿，胜利转进”一样的逻辑，空留后世笑柄罢了
</blockquote>


### 2020.10.27

<blockquote>
在农业时代，人的迁移只会从不能种庄稼地方向能种庄稼的地方聚集。在工业时代，人的迁移是从不能找到工作的地方向能找到工作的地方聚集。底特律的经验告诉我们，没有了产业城市就会衰亡。买房最重要的是什么？

</blockquote>


### 2020.10.22

<blockquote>

喂？报社吗？我，EDWARD LUCAS！
</blockquote>


### 2020.10.21

<blockquote>

那天王二正准备把剩饭倒进垃圾桶，只见阿猫用一种很可怜的神情看着王二，

王二试着把剩饭倒进了阿猫的碗里，只见它的尾巴顿时摇成了一个陀螺，埋头把盘子最后都舔得精光。
</blockquote>



### 2020.09.29

<blockquote>

然后我母上大人听到外面渐渐没声了，开门一看不见了人。

咬碎了牙，气炸了肺，追出去把刚刚走出楼洞的我给揪回来，进行了一波紧张刺激，生动活泼，感人肺腑地全面教育。

什么大慈大悲手，大仁大义脚，大爱无疆棍，时间太久已经不记得细节，只记得老妈一句十万分贝的狮子吼：“你还敢跑了！”


但是今天我都还记得我听到这句话时脑子里那萦绕不去的疑惑：“不是你让我'滚'的吗？”

...

性格 西江月 想找一个什么样的对象

对天痕怎么看

未来规划
</blockquote>


### 2020.09.28

<blockquote>

铁石心肠到底说说，人心还是肉长的，都有情感需求。我也真的希望回了家，能有人给自己一个大大的拥抱

...

当时只道是寻常
</blockquote>


### 2020.09.25

<blockquote>

那天，王二正走在走廊上思考着什么，突然学校里的恶霸老流氓跳出来堵在王二面前大声吆喝道：“好狗不挡道”

于是王二歪了歪脑袋，用一种疑惑的眼神看着对方，反问道：“那你为什么还挡道？”
</blockquote>


### 2020.09.22

<blockquote>

听了这句话，我心里的火“噌”的点燃了，我马上跑进厨房，拿了把菜d，然后跑出去比着她骂：“你他妈再讲一句？！再讲一句我就让你知道什么叫未成年杀人不犯法！”
</blockquote>


### 2020.09.21

<blockquote>

生活在这世界就挺麻烦，你不努力成为主宰，便老是有一帮龟儿子莫名其妙想要来主宰你
</blockquote>


### 2020.09.16

<blockquote>

明明自身趋炎附势，却偏要标榜文明道德。

...


全篇看下来

一个是典型的从小家里管太多，家长不自知，自己也不够有主见，等年纪长大些家里人不好管了，自己一下子想不出能干出什么事情来，只能很老套的叛叛逆，跟家里作作对...

书曾经能读好说明人不傻，可惜从小太乖太服从，独立意志、独立人格没发育健全，等到大了一旦找不到属于自己的事业、人生志趣，那么随着日子年复一年，便是蹉跎了岁月，内心麻木、空虚

他这嫖娼某种意义上讲不也是潜意识的想找刺激，试着刺激刺激自己麻木的心灵嘛


饱暖思淫欲，物质生活条件太好，生活太安逸，又找不到人生的目标，他只能打打什么 Dota、研究什么 av 中的技巧并实战才能维持得了生活这样子

什么？自己老婆总跟个木头人一样的好没意思、太没劲，满足不了自己？但是好想干那事啊！怎么办?！

什么？！兄弟们都常在外面找乐子，一点事没有？！

...


另一个带俩孩子是不容易，但很多甩手掌柜事情没亲力亲为过，不大可能会感同身受，去体谅当母亲的不易

但感觉楼主就是个内心很保守传统的人，思想好单纯，实际情况有些严重缺乏情趣，对男性甚至两性方面的知识缺乏了解，

摊上这种破事，处理也不够理性，本来就说是个内向的人，这种很私密的事情捅出去人尽皆知、颜面扫地，走在外面要被嘴碎的人指指点点，不管他当时做那事的时候心里有没有的愧疚感，如今心里会没点恨意、最后不整点互相折磨的事情幺蛾子出来？俺不信！单单冷漠冷暴力都算好了的


给不出好的建议，只能说多谈谈吧，互相更好地了解一下彼此，多鼓励鼓励让他找点其他自己想做的事情做，问问他要是这样蹉跎下去，老了回首这辈子，会不会有什么遗憾后悔


婚内嫖娼肯定不对，我一个阿姨以前也把叔叔逮了个正着，最后没离婚，过去了就过去了，四十之后还生了二胎的小妹妹，嘴上嫌弃经常嫌弃，但日子还行吧

实际上就算离了婚，结果又能怎样，让孩子变单亲家庭，从小缺父爱或母爱？或者二婚？

要么就打定主意以后不跟其他男人过日子了

不然，如果还在原来的城市、原来的环境，真的一下就能找到一个会尊重自己老婆、不会动手打老婆不家暴的老实男人？嫖资 2000 他完全可以不坦白，完全可以忽悠你

不仅不能沾黄赌毒，人生履历要清白，别女人太多，还得考虑啤酒肚、抽烟酗酒、打呼噜磨牙，最后生活习惯得磨合，更别提遇到的人真实品行是否端正，是否善于花言巧语...

...

对不起，不能加你好友

就事论事我多啰嗦几句吧

看你描述说明你在意他，并不真想离，但发生嫖娼这种事，太恶心，不能忍，心里真的好疙瘩，甚至让你忍不住开始猜疑，他到底过去还有多少这种经历瞒着自己，瞒着自己偷偷嫖过、约过多少回...

同时，这事闹得你们生活圈子里的人都知道了，绝对算是够极端，一般就像你说的，你男人颜面扫地了，不想见人，你发出去了，不离婚好像面子挂不住，会让人瞧不起


但是！最重要的还是看你们自己的幸福，这日子要不要过下去，怎么过下去，如果有挽回的余地，最后过去的就过去了，不用管别人什么闲话，俩口子自己日子过好了、过幸福才最重要


事情可以一步步来

只能说先别猜疑了，不然胡思乱想只会越想越恶心、越想越气

一种方式是，跟自己约定好冷静理性点，要是他能跟你老老实实地做忏悔，说出不管什么真相都首先不要太激动，冷静！克制！听他倾述！要不然，一听到什么就是对他一番羞辱，他还怎么愿意讲实话、继续跟你交流呢？最后只能选择用无言冷漠或者谎言代替

跟你先生好好谈一谈，说愿意听他讲，问问他那桩事情为什么非得嫖娼，嫖娼时候是个什么样的心路历程、对你可曾感到愧疚？

两个人能否一起做出些什么改变，他对你哪里有什么不满，你怎样能让他满意（说实话家务这种大多是女性在做，但是生活中如果两个人能一起分担，偶尔难得一方偷个懒，肯定是最好的情况）

最后也告诉他你真实想法，他这样子，你真的内心好矛盾、好痛苦，无法接受，很有可能一个狠心就真的离婚离他而去了，最好表演个声泪俱下，让他萌生怜香惜玉、恻隐之心...

问问他，他内心能接受最后离婚这种事情的发生、舍得你离他而去吗？舍得两个小宝贝吗？要是舍不得、接受不了这种事情最后的发生，那么让他思考一下，你们俩该怎么办...

很抱歉时间不够来不及写得更细致，主要是你得更加去真正了解他，具体方式你不妨思考一下


我会关注帖子，有机会再回复

...

没必要纹什么身，省得纹了后来嫌难看，偏偏洗来洗去又洗不掉，活受罪


“一个大老爷们什么样子嘛！娘娘们们的，担心这害怕那！你是那怂人么？！”

看到前面俺是真想说，尤其你先生这种温室里安逸惯了的，现在就是个会想太多但是行动太少的怂人，需要历练历练，你不必计较他的出尔反尔，而应该好好想办法鼓励一下，平常可以多说点类似“相信你自己”、“你行的”、“不要放弃”诸如此类的话

很多话他愿意跟你讲其实挺好的，但他想要改变可能就是得换个环境、甚至努力去掌握点专业的知识技能，现在开始都不晚，适当去外面闯荡闯荡碰碰壁，当然前提是家里有个好的港外，外面受挫折受委屈了，回了家要有个可以信赖的人，能够没有顾虑地倾述出来，然后继续闯荡，人一步步成长

至少俺见过一些家庭，过了蜜月期，有了娃，女方哪怕全职在家也会因很多琐碎的事忙里忙外、弄得焦头烂额，然后心情不好，而男方每天忙完回家，要么看自己的球赛拳赛，要么呼朋唤友打棋牌钓鱼，很多时候不爱跟老婆单独处，就是因为每次刚说出点什么，也不等人好好说完整，就被女方没好气地打断为难责难、各种贬低甚至辱骂，久而久之，很多事情还能聊吗？谁还吃饱了撑的喜欢自找没趣？于是少了交流，渐渐两人的心就疏远了

你可以回忆看看，你先生所指的不尊重不顾及，是否类似，或者下次意识到自己一个不小心说出口了，虚心点，问问他你那样说对不对，同时备个本子什么的记录一下


不要听了前面说的就觉得自己神经质、什么精神有问题

其实是这桩事很多人觉得不要紧，但对于你个人来讲，就是触犯、超越了你能承受的底线，太严重太让自己奔溃，变得歇斯底里罢了

真要算，可以说你还不够成熟、不理性，遇到这种事一开始没能够用更好地留有余地的办法妥善处理，直接是使出破罐破摔、用最坏的方式，而明明你说你的世界都是他，他有其他好的点，他也是自己追的你，并不愿意离婚

真的不妨搜一些讲两性心理、相处方面的书，对比下豆瓣读书上的评分评价，买来有空了看看，参考参考别人，反思反思你们之间过往的问题，不光对指导伴侣相处有益，今后也能更好地引导、教育自己小孩

不晓得你们那周遭环境闲言碎语、指指点点的风气如何，不如不好，现在这样的情况是可以考虑一下苏州，如果惦记家人什么的，现在通讯这么方便，多打打语音视频联系、有空多回家看望就是了

你也得用好的方式把自己真实想法感受好好表达出来，真正传达到他那，让他真的能理解到你，意识到问题的严重性，一起交流、认真去思考该怎样努力走出你们目前这样一个窘境吧


了解了彼此的过往后，人得向前看，该释怀的就得释怀，不能太计较执着过去怎么怎么不堪，如果真的能够你陪着他一起做出改变，往好的方向发展，那么当下和未来，才是最重要

...

不好意思，理解错了，原来你是指纹他身上

其实这种表面形式的东西意义不大，最重要的还是不能再让他觉得嫖个娼跟挠痒痒似的无关紧要，不要别人觉得嫖娼或者其他怎么怎么样，他也觉得怎么怎么样，不要人云亦云

得让他自己认识到你对此事零容忍、得让他有自己作为丈夫作为父亲的家庭责任感，绝对不能去沾黄赌毒、养小三

避免再结交会约他去嫖娼的人，别人家一喊，他就非得去，好像不去就很没面子很不男人似的

没自己主见、窝囊、不懂得该拒绝的拒绝、没责任心、不考虑家人，那才叫丢人

...

所以今天最后纹了么？说真的，尽量不要用这种一定得让他怎么怎么样的方式去证明他对你的感情，很不好，类似例子很多地方能找到的

倒不如跟他说可以不纹身、不结扎，让他先自己表态看看，犯这种严重错误，除了以后绝不能再犯，他自己打算怎么补偿你，让他自己去想，列个清单，你可以从中看看他的诚意，再考察他后面实际行动，看看他的态度，别太偏激


他所有朋友是他自己讲出来的吗，不然只是大多数倒还可信一些

但怎么说呢，这种就是常说的狐朋狗友吧

而且有一点，他自身有些思想观念上的东西要是不改变，可能不管到哪里，最后还是会去结交同一类的人

再好好交流看看吧

...

只看你描述，你老公不是那种完全无可救药、一无是处的人，但没主见、不够独立，朋友结交不好，便近墨者黑，所以局外人再帮你理理：

前面说过了，若一定要赌这口气，选择离婚，那么之后再婚？或者铁了心自己带孩子？

再婚未知数高，比你大的没碰过女性的男性几乎没可能，你介不介意？继父对孩子态度得看人品，人究竟怎样太随缘

若让你自己带孩子，前面你说“反正我就是那种不洗衣服不做饭基本不做家务的，有时候看垃圾多了受不了去倒垃圾”，人家一听会觉得你自己简直还是养在深闺中的千金大小姐一般，不禁要表示怀疑


打定主意暂时不考虑离婚，那就不要被其他人言论影响，没必要一条条跟人争论，思想上不要反复横跳，也不要因为之前发过朋友圈感到不离面子就挂不住，既来之则安之

但是你真得好好想想、规划规划，怎么给你先生来个彻底大改造，他被周围染缸染上印记，需要好好漂洗漂洗

还有你若只顾了自己感情感受，把你先生这么个已经有了俩娃娃还背着你聊骚、出去嫖娼的人一直放第一位，忽略你自身各方面心理、能力的建设、段位的提高，长远来讲，解决不了问题的

（甚至他签了协议还是屡教不改、屡教屡犯，最后不得不离婚，你至少要有能力处理家务能自己照顾、抚养孩子）

首先你至少不能太快原谅他

昨天看到“然后看到他又抱着他亲他，就是只要在一起我就的抱着他”这一段就特来气，傻女人嘛，那就像犯了错的小孩依然还被老母亲过分溺爱，小孩有恃无恐了以后不自觉地照样还会犯错

犯了错误就是犯了错误，要让他自己打从心底认识到错误，赏罚也要分明

这里贴个链接 https://www.zhihu.com/question/355677715

很抱歉不够了解你先生生平给不出好的建议，但是你不妨参考看看，甚至俩人一起看看

平常有空也多一起做点什么事，不管一起看剧看电影、旅游，一起打羽毛球网球之类的健身，总之多交流，增加些共同的经历、体验吧


...

但那个时候很少有人真拥有一台电脑——太贵了，动辄几千元的造价，足够工薪家庭挣几个月的了，大部分打滚撒娇要电脑的孩子，多半能饱尝一顿七匹狼腰带。
</blockquote>


### 2020.09.15

<blockquote>

雅思有个口语老话题，问你最喜欢哪个房间，

我学生人生忒无聊了，总是跟人家考官说自己喜欢书房，因为可以在里面看书，或者打游戏


你回答厕所嘛，你说经常在厕所里，坐在温暖的马桶上，点着薰衣草精油冥想，总是能神游普罗旺斯，或者在猫王复古收音机飘出的Louis Armstrong 沙哑嗓音中，回到早安越南罗宾威廉姆斯的怀抱

听到此处，考官不禁虎躯一震，惊为天人

...

此案发生后，____高度重视，立即召开____会议。____立即作出____，要求组织____，妥善处理___，迅速查清____，严肃追究____；立即组织开展_____，进一步做好____，防止_____。目前，____稳定。

...

某地搞军民共建活动，内容之一是纺织女工到军营给兵哥刷洗被褥。一位无邪的少女发现不少战士的被套上有一滩一滩集中分布的发硬的污渍，便不解地问俺同事是嘛回事， 男生咋也来月经？

俺同事沉吟良久方才答复：“您知道战士最宝贵的是手中那杆枪，他们晚晚都在床上擦枪，有时一个不慎就会把枪油滴在床上了。”  无邪的少 女深受感动，表示以后一定要向他们学习，象战士擦枪那样由衷地爱护自己的生产工具。 　

...

因为论坛的风俗是这样的：你和他讲数据， 他和你讲听感;你和他讲听感， 他和你讲单晶;你和他讲单晶， 他和你讲物理;你和他讲物理， 他和你讲英文;你和他讲英文， 他和你讲信仰;你和他讲信仰， 他和你讲医学;你和他讲医学， 他和你讲文学;你和他讲文学， 他和你讲修行;你和他讲修行， 他和你讲情怀;你和他讲情怀， 他和你讲道理;你跟他讲道理，他跟你耍流氓；你跟他耍流氓，他跟你讲法制；你跟他讲法制，他跟你讲政治；你跟他讲政治，他跟你讲国情；你跟他讲国情，他跟你讲接轨；你跟他讲接轨，他跟你讲文化；你跟他讲文化，他跟你讲老子；你跟他讲老子，他跟你装孙子！你跟他装孙子，他跟你讲道理….

...

什么？老大爷您尿频尿急？不怕，快使用我们这款，“量子磁场理疗项链” ，只要 1299 元！XXXXX ... 现在打折只要 799 就能买到，还送理疗磁石、刮痧板
</blockquote>


### 2020.09.09

<blockquote>

苦人的懒是努力落空了的结果。

苦人的耍刺里头含着些平等。
</blockquote>


### 2020.08.23

<blockquote>

我算是持中立，态度就像罗翔罗老师一样，要问我什么态度，老远的发生在重庆呢，我没有态度，这个评论也纯粹好久没写字了，写几个字练练手吐吐槽，结尾一段两个连问比较中二夸张，发的时候甚至在纠结删了是不是更好一点/狗头

要是生活中碰上，真有态度了，他老无赖是吧，想要这点医药费是吧，嘿嘿～


我们看到帖子的时间不一样，也特意回去了看下帖子，比方像你最初在那边 9 楼一码归一码、就事论事地写下建议、也提出自己的疑问就挺好，是老早已经看到帖子，而我看的时候下面评论已经 3 页多

我是基于相信楼主说的，大晚上的都十点半多了，肯定也是自己熟悉，知道一般没人来的草地空地，也像你所说，养过狗，知道自己狗的脾气性格，甚至像我，爱撸猫头狗头，从小到大各种猫狗小动物也都挺亲近的，有的看得出来，可以很亲热，有的离老远连我都不敢靠近，所以更想从只能在网上敲敲键盘重拳出击的老实人角度出发骂一骂那根据上下文判断出来想讹那 2000 快钱不想打针的臭无赖老流氓、讽刺讽刺那一些态度甚至人格都可恨的人


其实很多东西没必要讲，不论是之前余杭某（金发？）本地男子遛狗不牵绳、吓到人家孩子自己没点数还理直气壮下甚至反过来下那么重的手殴打人家妈妈，还是自己宠物狗一个不小心没看住结果发现被对马路的人活活摔死，以及那些无端虐猫虐猫甚至虐人霸凌性骚扰性侵犯，包括几天前老太的不幸、狗主人家的补偿对比那女孩及其家人若无其事的态度反应、老太家人的宽恕无奈，只要脑袋里没有因为各种自身的不幸、痛苦而导致塞满戾气怨恨冲昏头脑，整天到处批判这批判那，真的，正常有同理心的旁观者都能关注到那些事件的核心问题本身，不说是个个义愤填膺吧，至少也都能感受到那些都很过分、有违公德正义、充满问题

所幸的是，网上随他们键盘侠、随他们杠，只要事件爆出来了，现实中大都还是会有人去推动调查事情始末真相，一件一件地解决那些主要问题，最后处分的处分、该罚的罚、该判的判，虽然也有不少还没能解决，社会总还是有在一点点慢慢进步

最后一说这个也还是练手表达表达自己想法（哈哈），v 站现在也就不固定间歇性逛一下，本来前面写完就没考虑再回复了，之后都不回啦

换我，有话就好好讲，大家心平气和地就事论事，觉得对的可以坚持、错了就虚心接受和道歉，那点面子没那么要紧，如果遇上谁上来就各种问候、或者阴阳怪气地讲话人生攻击、哪怕涉及到祖宗家人，谁有理谁没理其实旁观者都看得清，我是觉得没必要去一般见识，甚至真实想法是：啊？就这？对唔住兄弟，俺没空，不鸟，告辞咯～
</blockquote>



### 2020.08.21

<blockquote>

“前两天刚面试了一所高校，当时院里领导问的问题就是怎么看待师德师风问题。

巧了么不是。

我的回答是，

我是从学生过来的，敬佩什么样的老师，讨厌什么样的人我心里是很清楚的。

以后如果真的有希望做一名高校教师的话，我不会让我的学生吃我受过的冤枉苦，遭那些本不应该发生的冤枉罪。

我是真心希望这种乱风气能够一点一点的向好，至少，我会从我自己这里做起。”

...

开始看到那帖子里楼主的描述，我首先想到的是西虹市里那个碰瓷的

说真的，如果楼主当时立马打电话叫来个什么身上纹着青龙白虎、脖子戴金项链的，你看那明显觉得楼主看样子老实普通好欺负的碰瓷刁人老无赖，还敢不敢再多一句咦咦啊啊、搞七捻三，早就秒怂吓得一库马赛跑路了


然后看到下面评论就挺无语的

有人提出绳子不牵，后面的评论直接主次不分，风向带歪

这就类似之前很多的案件，比方明明是某人强奸幼女或者某些女性遭刁人侵害引起讨论，往往开始众口一词，都站在道德高点骂嫌（实）疑（锤）人（者）

可中间一旦谁有意地给你丢出些什么证据信息，部分人的反应就非常有意思，会觉得，哦，这个女的恐（肯）怕（定）也不是什么好东西，要是再有什么职业水军之类的人给他们起个头，真会有人开始认真地参与起人家水军的工作，给人打起白工来还不自知，甚至更夸张、更憨批一点的，一本正经地分析起所谓证据信息，给你来一篇类似题为“从XX分析XXXXX（不是好货）”的长篇大论，真的是人云亦云，脑子比我还不清不楚，净瞎掺和

其中也有不少人，最可恨最讨人厌，是那种一旦抓着别人小辫子，会一副盲生发现了华点的样子，非常自鸣得意，之后喜欢显摆出一副得理不饶人的丑恶嘴脸，搞得来好像他们自己道德有多么高尚。往往就凭他们最初的那副道貌岸然，和之后的各种粗鄙之语，一对比，真的不禁要让人想这些家伙怎么也不先自己掂量掂量，别人听着看着都觉得怪害臊的

不管那个带头的人有意无意，这不就是转移问题、转嫁矛盾嘛，像什么trump政府、有些游戏的官方，就都挺喜欢用，可明明一切一切的起因是有个最主要的问题实实在在摆在那里啊！拜托有谁重视一下？！有谁解决一下？！

...

王二后脑勺某名奇妙挨了一下，便撸起袖子要打架，等站起来发现人家高自己一头，便（跟个 XX 模仿的汉奸那般）赔笑道：

“大哥误会、误会啊....天太热，袖子上都是汗。”
</blockquote>


### 2020.07.27

<blockquote>

愿意听听我说么，

那天我问去无锡能不能见到你，你说必然见不到，我没有多问为什么，也许你是在开玩笑，又或许你是说真的，但我是猪头三，我没法知道。

我只知道自己挺绝望，
</blockquote>


### 2020.07.23

<blockquote>

儒家吃人，不能算吃人，读书人的事...接连便是难懂的话，什么“汉贼不两立”，什么“贼不算人”之类。
</blockquote>


### 2020.07.13

<blockquote>

ʕ•̫͡•ʕ*̫͡*ʕ•͓͡•ʔ-̫͡-ʕ•̫͡•ʔ*̫͡*ʔ-̫͡-ʔ
</blockquote>


### 2020.17.12

<blockquote>

我们说 一眼望穿的未来最为无聊

嬉笑打闹 随性生活的那段时光

啊 真希望当时能懂得

一旦离开

就再也回不去那个地方
</blockquote>


### 2020.07.10

<blockquote>

铲车人问禅师：戴java技术怎么样？

禅师不语，只是将手边的一把斧头狠狠地砍到了木桩上。

铲车人大喜：戴java技术入木三分？

禅师缓缓吐出两个字：劈歪

...

桑桑的母亲知道桑桑有了下落，心里的火顿时又起来了
</blockquote>


### 2020.07.08

<blockquote>

“王二，我要摸你头！”“？？？还来？这次手头有什么！？”“一块糖行不行？”“行！摸吧！”

</blockquote>


### 2020.07.06

<blockquote>

“像《神秘海域7》这种游戏，它拥有不亚于电影演出的效果”
</blockquote>


### 2020.07.03

<blockquote>

七年啊，什么概念？基本上在漫漫的历史岁月长河中，如沧海之一粟，不值一提，可对于个人，说不定就是整个青春年华、整个黄金岁月，有可能经历相当多的人和事。不晓得还有没有人记得之前高中毕业典礼时被我带去的那个和我拦腰高的小鬼头，转眼也已经上完了初中。中考成绩出来了，她的家人和老师统统想不到，这个准新东方准蓝翔学员，居然考上了那所高中，老哥和老妹，以后又成了校友。
</blockquote>


### 2020.06.22

<blockquote>

“老师老师，它这里面有描写中国与北约的全面战争，很真实很震撼的，这人是不是真打过仗？”
</blockquote>


### 2020.06.16

<blockquote>

所谓错误的前提导致错误的结论，新手用 Hook，不去看最佳实践，相关语法约束，啥鬼代码都能给你写出来
</blockquote>


### 2020.06.07

<blockquote>
56772 3549 807

56552 3698 810


60642  5282 1177
/api/v/live/${ window._stableLiveId }/purchase/jsapi/ 微信内（公众号）支付下单

/api/v1/live/${ window._stableLiveId }/purchase/web

/live/:liveId/purchase/status  查询购买状态

/api/v1/live/${ window._liveInfo.id }/purchase/free 免费




咋和那小子分的手？他妹说这不寒假两个月见不着面，没感觉了呗。等到后来开学，两小鬼头你侬我侬，王二无语
</blockquote>


### 2020.06.03

<blockquote>

为了响应国家号召，王二最近淘好了一批货，在余杭塘河的某桥头摆起了地摊，手拿喇叭高声喊：“阿妹力卡黑人兄弟现抢，梨头手机九十九块八，VL 包包九百九十八，劳氏力一千两百九十八，数量不多，先到先得！”
</blockquote>


### 2020.06.02

<blockquote>

尤其中间这一段叶文洁被捕，加上那游戏什么的，都挺扯淡的

就像常规的电影里反派大 BOSS 明明可以在后台，偏偏亲自出来自动解释来龙去脉
</blockquote>


### 2020.06.02

<blockquote>

他说，她那没有女人味的女人味，反倒深深吸引了他
</blockquote>


### 2020.05.27

<blockquote>

“以此为骄傲，是实在没别的可以骄傲。”

—— 沃兹基·硕德

十年前被判冤假错案的王二在月初总算改判无罪给当庭释放，之后还到账了一笔数目不小的国家赔偿。

接回家休养了这一阵子，王二的老母亲一边忙着给他在同小区看二手房、签合同、过户交割，另一边已经托人联系安排好了一场相亲。

只说那天去相亲，
</blockquote>


### 2020.05.20

<blockquote>

没文化又没历史太可怕了！

川皇这是和袁本初一个思路啊……

本初不就是觉得献帝没兵没权，养着费钱费粮不说，还添麻烦嘛！

谁知道阿瞒捡到献帝后来了个“挟天子以令诸侯”？

“得道多助，失道寡助。寡助之至，亲戚畔之。多助之至，天下顺之。以天下之所顺，攻亲戚之所畔，故君子有不战，战必胜矣。”——《孟子·公孙丑下》
</blockquote>

### 2020.05.19

<blockquote>

真无语。搜 module federation，出来一堆针对同一篇官网原文的翻译，就换了标题挂那边骗流量，还不如看源码

...

事情是这样的，王二是个程序员，那天他在查 module federation 的相关资料，
</blockquote>


### 2020.05.15

<blockquote>

愿中国青年都摆脱冷气，只是向上走，不必听自暴复自弃者流的话。

能做事的做事，能发声的发声。有一分热，发一分光。

就令萤火一般，也可以在黑暗里发一点光，不必等候炬火。


此后如竟没有炬火：我便是唯一的光。倘若有了炬火，出了太阳，我们自然心悦诚服的消失。

不但毫无不平，而且还要随喜赞美这炬火或太阳；因为他照了人类，连我都在内。
</blockquote>


### 2020.05.14

<blockquote>

那天早上王二艰难起床，一如往常感到胸口隐隐作痛。

待洗漱完，正要出门，屋内突然伸展开一个空间裂缝般的东西，里面跳出一名似曾相识的女性。

王二还来不及开口，对方便已经走到王二面前，抬起手就是一巴掌，留下一句“再熬几天夜，你不用做人了”，就回去随着裂缝一起消失了

...

（槟榔）这玩意，运气好毁容，运气差火葬场
</blockquote>


### 2020.05.11

<blockquote>

我看着他们满怀羡慕

影院积攒几年的财富

所有的场地、座椅、投影仪和大荧幕

像是专门为他们准备的礼物

...

毕飞宇在访谈中讲过一个非常类似的故事：

一天，一位穿喇叭裤的小伙子上了船，另一位没穿喇叭裤的小伙子动手打了他，

被打的小伙子问为什么?

打人的小伙子大骂道：“老子就是看不惯你穿喇叭裤的样子！”


两个小伙子被拉开后，船舱里的人开始讨论，讨论的中心是 —— 小伙子该不该穿喇叭裤。

没有人讨论，小伙子该不该被打。
</blockquote>


### 2020.05.10

<blockquote>

王二新认识了个朋友，在她家，他看着墙上的那幅画，她介绍说那是她爷爷遗像，听说在她出生前被人蘸酱油吃了
</blockquote>


### 2020.05.09

<blockquote>

“现在的人都只能同甘，不能共苦”“话不要说这么绝对嘛”“那你给我找一个？”“这点抱歉，俺是独身主义”
</blockquote>


### 2020.05.06

<blockquote>

遇见中意的不免处处小心谨慎，遇见对自己有好感的往往有恃无恐，虽然做法不值得推崇，实乃人性使然

...

近之则不逊，远之则怨，不只女人小人，世人皆如此
</blockquote>


### 2020.05.02

<blockquote>

那天吃过午斋，王二突然有兴致给张三聊起了自己出家前的一点事。

王二说自己有过一个从小一块儿长大的表妹，记得那年端午前，在他扛着麻袋赶往大巴站的路上接到了他那个表妹的来电。

聊着家常，王二问他妹近来生活可好，她想了想，说有件事情准备告诉他，听了可别惊讶。

他听闻此言，在电话这头问该不会她已经被猪拱了，而电话那头也同时把这件事说了出来。那一刻，她笑得花枝乱颤，可害羞了。

人类的悲欢可并不相通，就在同一时刻，王二的心隐隐作痛，想到了他舅，提前体会到了不久后的那个夜晚，他舅将感受到的那种好不容易养大的白菜，就那么被猪给拱了的心绞痛。

第二天，王二去外婆家做客，见到了他妹。他妹以难得跟他一同出去玩为由，拉着他一起去见那位。

等见了面，嗯，高高瘦瘦一小伙子，王二抬手跟对方打着招呼，同时，那种白菜被猪拱的心绞痛，来得更加强烈了。

那天之后发生的事，王二直到今天也想不明白。

见面前，他妹跟他介绍说，两人刚确定关系不久，是她表白了那个人，而那个人本来也正准备跟她表白，她说那人之前身边女生不少，自称有点像石头记里的那个王二？


</blockquote>


### 2020.04.28

<blockquote>

她听闻前男友死讯，尸骨无存，便在家里做了个佛龛、摆了个牌位，还拉着我天天祭拜，初一十五还要吃素，妈耶

...

阿姨说，这娃应该是他爸喝了酒造出来的吧。智商低。

...

我的天，你们听到了吗，她竟然叫我哥哥！而且声音特别的甜美，现如今很难找到长相和声音一样甜美的妹子了，而且此时此刻就坐在我的面前。

之前我特别反对这种带有封建主义色彩的相亲活动，如今发现还是我太年轻，没有认识到中华民族文化的博大精深，既然是存在的，那么必然是合理的嘛，实践是检验真理的唯一标准！

...

“哈？你怎么又把钥匙给忘了！唉，我都跟你讲过多少遍了！好，我马上来！”“对不住，我先走一步，失陪！”

</blockquote>


### 2020.04.27

<blockquote>

<!-- 这两年新闻之类的比以往接触的多了，看着不少人和事你方唱罢我登场，挺有意思，但其中随便一件要是发生在自己身上 -->

...

真诚交换真诚，礼貌交换礼貌，可惜在网络上迷失的人，一边自身匮乏空虚，痛苦至极，一边又大肆投入到廉价的网络活动中，抱着敌意的生活社交，彰显自己的存在感，却连自己缺的是什么都不知道。

...

“小兄弟，人家制作人员那么久的打磨你以为是瞎搞吗？”
</blockquote>


### 2020.04.24

<blockquote>

其实以后招实习生在最后环节聊一聊个人平常技术方面遇到问题，都是怎么去解决，可以例举一个王二或者张三，说这兄弟不管遇到什么问题，首先就是问人，自己也不去想、不去搜，你怎么看，主要看他以后在公司，问别人问题前是否偏向于自己先动动脑筋

还有如果加班或者不加班，可以一开始就说清楚，顺便也询问，如果平常其实是不用加班的（前提条件，划重点），但偶尔真的遇上问题来不及解决，能否接受至少走之前尽可能把自己的问题解决掉，不给人添麻烦，最主要看个人是个什么样的态度，会不会一看到这个就想到说什么 996 啊没人权、无法接受

...

js ≈ 走路、jq ≈ 骑车、vue/react/ng ≈ 开车

- 如果终点很近，当然是随便怎么过去，滚过去都行

- 如果终点很远，当然开车最快。反对开车的理由实在有点搞笑

问：不会开车，等我考完驾照再来开，我单车都可以来回十趟

答：如果只去很少的次数，当然没必要学新的东西了

问：开车效率低，不如我单车可以选最短路

答：路程短，时间不一定短。小路也不怎么安全

问：单车维护成本低，容易修

答：所以选工具最重要的因素是好修么？

问: 开车烧油，消耗大，不环保

答：如果你真的这么在乎这个，那就慢慢骑车吧，还能锻炼身体。只是等你去一个地方的耗时，人家可能已经来回十躺了

当然了，有些极端情况确实没法开车，比如路太窄、道路禁止机动车出行、乘客晕车等
</blockquote>


### 2020.04.17

“请问你最近有什么打算？”“呃，打算嘛，俺这不最近把地中海剃了个光，正好可以回天台山找老师傅收留”


### 2020.04.15

<blockquote>

爱情这种东西太奢侈了。年轻人有自我职业技术追求，得投入大量时间静心专研，想找个能支持自己的爱人不容易。

</blockquote>


### 2020.04.14

<blockquote>

留言说一下吧，昨天看有人帮内推我就邮件给了他简历，其实也是瞎投，虽然有点不好意思，

我这边都是可以的，就是得跟之前那位邮件说一下，麻烦他撤销一下，

我因为对这个内推流程不清楚，刚才有点不知道该怎么回复你。我之后给之前的联系人发了邮件，拨打了热线撤销支付宝的投递，说是三个工作日内给予反馈，等反馈出来我再通知你？这里也想顺便一问你这边的业务，等下班空了有时间回复我吧。无论如何，有劳费心了！

...

实在是不好意思，中午我同事联系了他在阿里的前同事帮忙内推，但因为先投递了你这边，导致他那边没办法提交。

我可能也不是特别满足支付宝这边的岗位对移动端方面经验的要求，所以能否请麻烦帮忙撤销一下我前面的这份投递，太麻烦你啦！
</blockquote>


### 2020.04.13

<blockquote>

呃，不管前端后端，掌握特定语言是最基础的，之后学习实践的过程中还需要积累特定应用领域的领域知识

比如前端我要写 PC Web 网页，我除了得掌握 html、css、js 语法，还得了解 DOM、WebGL 有那些 api 可以用，之后怎么通过 js 来组合利用？

要写浏览器插件，我得了解 chrome 的 api，比方要获取标签页信息、要实现页面和 background 的通信，都能够用哪些 api 来实现需求？

用 Electron 写客户端程序，用哪些 api 怎么来完成 ipc 进程间通信？

之后遇到需求要实现的各种模块组件，让我自己来，该怎么写呢？再之后，为什么目前实际工作中开发，肯定得用 React 或 Vue 或 Angular 这些框架，它们本身都解决了哪些问题，给我们的开发带来哪些便利？

还有什么文件的编译打包，npm 上的各种包，太多啦！

当然还是积累不够，真想要入行，肯定得一步一步脚踏实地慢慢积累
</blockquote>


### 2020.04.10

<blockquote>


愚道前辈，你好，我是昨天那个电话面试者许天柱，不好意思希望能占用你一点时间多少请教一下。我还是很想了解下昨天面试你这边大概是怎么个评价，比方说我技术是否能过关，可不可以尝试继续投递其他 P6 的开发岗位，

又或者昨天电话里讲话嗯嗯啊啊结结巴巴的（当时我应该先倒杯水），说明我这人思维混乱、逻辑不通，P6 也是实在太不合适，那真没办法，在下只能告辞。

昨天电面完我去看了官网，才意识到这个职位投递肯定是有问题，标注着“资深/专家”的字样，我最初只是看到要求“3 年以上”，是“体验技术部”便投了。

现在想想，“资深/专家”简历居然能过，还给了这么久的电话面试，而最先在 antd 官网的“加入我们”给 afc163+antd@gmail.com 的投递前端工程师岗位邮件至今没有任何消息，有些预料之外。

我看网上有说，阿里内部面试评价数据都公开透明的，如果昨天评价已经够差记录在案了，那我继续投递肯定是多此一举了。

还有当时问到绩效职级，我说一般般，不知道这个影响大不大，当时其实是没好意思直接说同事、主管评价我算目前花瓣前端主力，尤其现在人少，项目的前端多是我在负责，本来早就说评级涨薪，奈何花瓣现在被版权的官司纠缠，以及受这次美股影响，谈好的的融资断了。

最后问到个人优点，心里话挺难说出口的，只能大概说我一直自诩以兴趣为职业，求知欲强，是个终身学习主义践行者，爱看那些经典的小说杂文，平常自己写点比较虚构扯淡的小短篇，在技术上也有自己长远的目标追求。

我好奇如果当时电话里如此讲，评价什么的会不会好点，当然也有可能这些其实影响不大。

毕竟在花瓣呆了这许久之后刚开始尝试投简历找新工作，头一个电话面试嘛，希望能从这里获得些真实反馈，为之后的求职，吸取些教训。

本来想过 12 点之后直接打个电话问一声，但想想我平常都是沉默寡言，多少有些口齿不清、最后会讲不拎清，自己其实也不大爱接陌生人电话，所以还是发邮件吧。

肯定还是希望能有回复反馈吧，不论如何，非常感谢。
</blockquote>


### 2020.04.09

<blockquote>

我刚才笑得肚子疼

小月欣你这人有时候好好猜好好玩

我刚发完表情，就已经猜到你将会回我这个表情
</blockquote>


### 2020.04.02

<blockquote>

"What happens when it happes." 我的天，这人简直哲学带家，堪称当代老子
</blockquote>


### 2020.03.28

<blockquote>

非常感谢回复，同时不好意思，回复得略迟了，因为自己刚开始准备求职，很多东西没有复习整理过，早上看了看，挺凌乱的，一时不知从何说起。

我这份在线简历里链接了的网站都是自己这边公司的项目，本来想如果有需要，直接在微信或者电话又或者在 Slack 按照具体项目具体的点试着讲些项目经历。

其实在 github、v2ex 账号以及 slack、微信用的昵称同样都是：igoist


github 地址：https://github.com/igoist

我这边简单讲几个：

https://github.com/igoist/Web

这个库算是我比较早期的练习集吧，

如 draft，里面是实现一些看到或者想到的东西

demos 类似，相比 draft 里面按照元素组件类别有做整理

有写简单的 README.md，里面大多可以在 git clone 下来后丢到 apache 配置的目录或者直接丢到浏览器访问，还有些可能需要进去编译下 style.scss 甚至 npm、yarn 下载依赖


https://github.com/igoist/Config

这个这里也顺带一说 我自己编辑器、shell 的一些配置


https://github.com/igoist/plugin-IAdB/blob/master/src/oneForAll/oneForAll.scss

一个简单的浏览器插件，可以改网页背景色、屏蔽或调整一些网站的内容，链到了 .scss，可以参考我常用写法


https://github.com/igoist/erb-ui

一个 18 年开始整理的 React 的 demo 练习集吧，有时候想到，或者项目中需要的页面、组件，会写在这边，不过这个大概太凌乱了


https://github.com/igoist/color-picker

简历中那个客户端拾色器源码，本身是放在前者 erb-ui 下 src/usecase/ 目录下需要配合启动的


https://github.com/igoist/ts-boilerplate

在我的 github 中搜 boilerplate 关键词能搜到好几个，是以前边捣鼓 webpack，边整理自用脚手架，如今实际做项目，还是蚂蚁云谦写的 umi 好用


https://github.com/igoist/TmpReview

一个建立在 umi 基础上近期项目中临时用的评审后台


别的这边也不多说了，确实挺凌乱的，有时间可以看看这些项目 src 下面具体页面里一些写法，以及参考 public/sass 下的内容

同时我也继续整理，如果有下文，希望再详谈吧


--


Thanks!
- Warald

</blockquote>


### 2020.03.27

<blockquote>

用 React 开发 Chrome 插件，能否配合 HMR


起因是前面看了两周 Pinterest 那个插件的源码，晓得了像它和 cVim 这类都是在页面中 inject 一个 iframe，里面写了一堆逻辑，和 background 通信来通信去，

期间自己也边看边在写 demo 踩坑，试用一些 chrome 的 api，比如 iframe 中执行的 js 文件，可以直接像 chrome.runtime.sendMessage({ to: 'bg', via: '?', payload: {} }) 这样调用，

于是想到可以把自己写的一些工具搬上来，再把原来写的一些插件重构下。

现在主要问题是，最初想直接套 umi，在 localhost 某

</blockquote>


### 2020.03.23

<blockquote>

“起码比看那群蠢人演的电视剧好嘛，你说颜值也不高，台词严重脱离生活，我看了都觉得对我智商是一种侮辱”

...

这也难怪，毕竟活人更在意“这场丧事办得闹猛！吃得惬意！”很少回头去追问死者“你活着时儿子对你好不好”。
</blockquote>


### 2020.03.20

<blockquote>

婚姻是一把伞，而人生大多数时候是晴天。
</blockquote>


### 2020.03.13

<blockquote>

虚假的中立国：别人打架我绝不插手

真实的中立国：别人打我我没法还手

虚假的中立国：你们打，我就当什么也没发生

真实的中立国：你们打我，就当什么也没发生

...

嘴巴那么毒，内心一定有很多苦吧

so much spice, so much pain
</blockquote>


### 2020.03.06

<blockquote>

懒汉王二以前都是随机不定期偶尔下厨瞎烧点东西，知道自己大有问题，比如搞不懂火候，该放多少油盐酱醋，但不求甚解，不做功课，又不大在意，自然也常粘锅。

可王二最近除了恰饭睡觉去菜场捡菜叶，便是回桥洞洗菜切菜淘米煮饭再刷锅洗碗，天天如此，烧的回数多了，不免经常要粘锅，偶尔还粘得特厉害，不用热水泡，怎么也刷不掉，不免搞得王二头皮发麻内心备感挫折。

正所谓痛定思痛，这次王二终于铁了心，决定发狠去搞明白个所以然。

一查，据原物理带师王师傅王二口头翻译复述，锅在显微镜下，其表面原子还是分子结构单元会有个缝隙小孔，粘锅很大程度上是食材的一部分嵌入了一个又一个孔，要是能够让油分子充分填充这些小孔，基本上便阻隔了食材与铁锅表面直接接触，避免了食材嵌入小孔。

此外，清洗后的锅如果倒油前不充分烧干，水分子会占据前面说的那些小孔，使得密度低于水的油分子难以进入，再经过翻炒什么的一来二去，食材就会进洞导致粘锅。

最后，为了向记者观众证明自己这次也是实话实说没吹牛批，此前逢煎蛋必粘锅的王二特地捡起砖搭起炉灶，放好柴片生火，把清洗后的锅烧了个通红，再倒入少量油，拿出那个被他捡来珍藏了许久的鸡蛋，眼神略带不舍同时看他手有点哆嗦地打了蛋下锅。

咳，别说！王二这回倒是真没吹牛，真被他有生以来头一次的煎了个完好的流黄蛋出来，同时看上去似乎一点都没有粘锅。
</blockquote>


### 2020.03.04

<blockquote>

这些天各个企业都在陆续开展复工相关事宜，王二的公司也不例外，要求刚返喀什的员工们先在住处隔离观察，远程办公一周，可这才几天，王二又被炒了鱿鱼。

这次是这样的，人事部门要求所有远程办公的员工每天傍晚提交一份日报，按说如果真没东西写，随便扯点慌写上去也就得了，可憨憨王二偏不这样，在头天的日报中老老实实填写了以下内容：

09:00 - 09:30 做早餐吃早餐

09:30 - 11:10 发呆梦游

11:10 - 11:45 淘完米，去菜市场采购并返回

11:45 - 12:30 煮饭，洗菜，切菜，炒菜

12:30 - 13:00 恰饭

13:00 - 13:20 收拾，洗碗，刷锅

13:20 - 15:45 饭后休息，之后睡午觉

15:45 - 18:00 喝茶发呆梦游


本来这日报人家人事也就形式一下，进行个别抽查，你不想写，人家人事负责这块的人更不愿意看呢。

只是那天周四刚刚刚刚刚好，人事主管闲着没事情干，在邮箱中点开了名为王二的这名员工的日报邮件，看到了如上内容，便皱起了眉。

人家通过检索，再看了王二另外两天的日报，内容也是诸如此类，便感到又好气又好笑，当即决定上报。

不需要经过什么讨论，上头一致通过决定，开除了该名员工。

这也是为什么此时此刻，外边寒风料峭，细雨飘飘，而王二却在车站台扛着麻袋、等着大巴，两眼呆呆地望着远方出神，不晓得会在想些什么。
</blockquote>


### 2020.03.03

<blockquote>

他是说父母在，你总会觉得有依靠。到后面就只能靠自己的时候，大概才能体会真正的成长。

...

生活上独立，不再依赖于父母。

开始承担生活中各种角色所赋予的责任，比如：作为年迈父母的儿子，作为妻子的丈夫，作为小孩的父亲等等。

对于任何事物，都有着自己的看法，对于不理解的事物，会先小心求证再判断，不人云亦云。

承认自己的不完美与平庸，但不放弃提升自己。

开始理解，“舍得”这个词的含义，懂得知足。

...

一月的蝙蝠，二月的鸡，三月我们变穷B，年前一毛没剩，年后一分没挣
</blockquote>


### 2020.02.28

<blockquote>

年前曾默默许愿，希望能放下手头所有工作，给自己放一个长长的假，好弥补一下那些自己欠缺的知识，调整调整作息，看几本自己想看一直没来得及看的书。

按说除非离职待业，或者是选公务员、教师这类职业，不然工作后，几乎就不可能再有学生时代那种长长的寒暑假。

万万没想到的是，春节期间一等再等，延期复延期，最后某种意义上来讲，那个几乎不可能的愿望竟然因为这次这个突如其来影响会后世的疫情而TMD给实现了，见了鬼了。

就结果来说，噗，说出来也是真丢人，自己每天跟个猪头三一样吃了睡，睡了吃，资料文档没怎么看，代码没怎么写，书也只不过看完了随身带回了家国庆B哥也买的那本小黄书《霍乱时期的爱情》的最后篇章，倒是又追了不少动漫，看完了木鱼水心推荐的那部《请回答1988》，还看了不少冷面魔男铲车人领袖戴Java玩炉石、三条路、恐怖游戏实录。

再看歪研会，看同龄人高佑思，想到更多新闻中被报导或未被报导、承担着风险工作在一二线的那些人就感觉自己也真是惭愧，只能整个月地宅在家算做点超微薄的贡献。


还有想说的，就像养小孩，差不多大的时候就该放手让孩子多去爬、去自己跌跌撞撞地学走路，一路上免不了要受点苦，可没办法，如果一直裹在襁褓中，永远学不会走路。

人之后的成长也是，一路上，有些事比如黄赌毒绝对不能碰，但还有些事是需要鼓起勇气迈出步伐努力去尝试、去经历的，尽管挫折、苦痛往往不可避免。


眼看着马上复工了，希望接下来的一年里，能一项一项地完成自己的事项清单，先调整好作息，每晚几点后告别屏幕，早睡早起，做好自己想做该做的事情，在这种黄金岁月里去努力证明一次自己，实现跟阿金提过的三年之约，早点把日语掌握，周末也多做做饭，或者多出去出去结交些新的朋友，而不要像以前那样一年到头宅着，浪费西湖边这么好的地理位置资源。

也祝愿那些没来得及问候的同学老朋友们新的一年里诸事顺利。

...

最近迷上了一首国漫里出现的歌曲《连备胎都不是》，不知为何，其歌词，其旋律，扣人心弦，直达我的灵魂深处

...

逃脱 不想面对我的错 承诺给的多 已失去自我 我只想要 逃脱 避开不必要的错 我就要慢慢摆脱 爱给的泡沫
</blockquote>


### 2020.02.21

<blockquote>

王二外甥网恋记：

那天一大早王二接到他姐电话，说晚点要带着他外甥过来，希望王二帮忙开导开导。

王二心里还正纳闷着是又出了什么幺蛾子，嘴上却已经在连连应承“好的好的”。

等挂完电话，王二一面给媳妇汇报了此事，拜托她这位特级厨师能劳烦中午下厨随便露几手，一面抄起口罩证件急急忙忙下楼买菜去了。


快中午时候，王二正给铲姐打着下手，电话响了，王二他姐说到了，他便前去开门迎接。

王二跟阿姊打了招呼，再看外甥，只见外甥强颜欢笑着跟自己问好说“阿舅”，愁眉不展、一副生无可恋情绪很低落的样子。

之后吃了饭，稍微聊了会儿天，等王二他姐回去，再跟媳妇眼神交流完，王二把

...

兔子与月亮这个故事的一种解释是：患得患失，迟早得学会放下

...

即便饭菜很好，心事重，没地方说，老母亲问儿怎么没胃口，只能推说人难受，明明第二天又要分别，太难了
</blockquote>


### 2020.02.17

<blockquote>

事情要从那次王二建议他那个快三十岁却都还没谈过对象的外甥王小锤对象

...

小月欣昨天肯定看到消息的吧，为什么又不回呢？是觉得无话可说，还是嫌天痕烦？他心里好多问号，什么时候能跟他好好说几句吗

...

人生啊，是这样不可预测，没有永恒的痛苦，也没有永恒的幸福，生活像流水一般，有时是那么平展，有时又是那么曲折

高加林最后放声大哭时，哭声中有对刘巧珍的感激，有失去巧珍金子一样的心的懊悔，但更多的是对人生的无奈。
</blockquote>


### 2020.02.11

<blockquote>

有很多本可以凭自身努力完成的事若没来得及实现，便无法再与外人道，要么选择花时间努力，要么默默遗憾放弃

...

流浪老汉王二在2020年初那场后来当时轰动全球的疫情中中了招，
</blockquote>


### 2020.02.08

<blockquote>

霸天铲、既生戴何生铲、复铲者联盟、铲头强、放开我来铲、妇铲科医生、长大了我要开铲车人、麦克佐铲、有铲阶级戴佳玮

我是铲车王、炉石第一铲子嘴、老鹰铲小鸡、西门吹铲

环境不错、民风淳朴

为所欲为铲天柱

...

（上了个咆哮魔）亲自出马

...

游戏不好好看，一直在那里变形变形，变你个大头鬼

...

“那我如果刚才直接打个咆哮魔，吃个爆裂符文，当有人骂我彩笔的时候，你是为我说话，还是在后面擂鼓呐喊呢？这个问题就来了，对不对”

...

想死是不是、你疯了吧、不要去

</blockquote>


### 2020.01.2x

<blockquote>

王二约了阿杰出来当自己亲友团去和本地女网友相亲

...

清了几次嗓子，王二终于走上台，说道:“人嘛，别当连自己都讨厌的人，再努力争取成为自己想成为的人”
</blockquote>


### 2020.01.20

<blockquote>

这位小伙子站起来说各位领导各位同事，我有个事情想和大家探讨一下，想听听各位领导和大家的意见。大家都知道我的女朋友是XX部门XX，最近她经常被各部门领导叫去参加各种迎来送往，还经常被灌酒，我有几次在酒店门口等到12点才醉醺醺出来。

XX刚毕业，一点酒量也没有，也不善于迎来送往，更不属于工作范围，请问各位领导各位同事，如果你们的女儿或者妹妹遇到这种情况怎么办，你们眼睁睁地看着刚毕业的女孩子被各种灌酒被各种黄段子包围怎么办？我想听听大家的意见，我年轻，我想知道拒绝不属于工作范围内的事情会不会被打击报复，反正我看了好多官场小说都说会这样，但我相信咱们局领导都不是这样的人。
</blockquote>


### 2020.01.19

<blockquote>

是我当时太乐观了吗？我质问我自己，但是现实是当时的我啊……

用我这辈子最温柔的声音说，不论你什么样，只是见一面，没关系的～

嗯我想回到过去抽死当时的自己，

然后远远地……远远的……我看到了一个能把我车胎压爆的妹子，她就好像把我给她买的零食重量，全部加在了脸和腰上，一个女孩子会有小肚子……

其实微胖很可爱，但是她那个肚子，我在某孕育医院经常看到，一般这样的肚子，三个月后都会喜提孩子，但她通过自己的努力，不需要我播种，天赋异禀。

不是潜力股那种，大概率瘦下来也不会好看，我虽然是宅男可是平时也是有注意体型的……。

吐槽了这么多，只能说明我是个颜值党，是个看脸的渣男，我在驾驶座上呆滞了至少有三十秒用来确认到底有没有看错，长呼了一口气我也不知道我脑子为啥抽了……下了车。

下车她呆呆地望着我，我比她高一个头，然后!

没有一点征兆，她扑了上来抱住我的腰!

火影里面那个丁次的肉弹冲击，或许也不会比这强太多吧我真是个强大的男人啊。

来不及感叹了……

之前说好的害羞呢喂!

然后就是一段我不想回忆起来的尬聊

她羞红着脸

我半扶着腰

全程把着车门，

生怕她那肥硕的腰身用一种极为灵活的方式挤进我的副驾驶，我怕安全气囊会马上弹出来，我怕我见不到明天的太阳。

她:芋芋，你还长的还挺高的

我:那个你其实……和照片上不太一样啊哈哈

她:其实是P的，最近吃的比较多……我瘦下来就是那样子的……（委屈巴巴）

我:……

她……（扭捏）你……

...

先说结果：据景区一名工作人员透露，这头猪当天蹦极完之后，就被当做年猪送往了屠宰场。
</blockquote>


### 2020.01.18

<blockquote>

这个王二所在的世界的审美观与其他世界都不太一样，按说其他世界中，一般都认为身材匀称、五官端正是好的，

而像王二这种大老爷们身高 160 公分、体重 163 斤，就显得又矮又肥胖，说得不好听点，简直就是个柴油桶

...

是吗，我失恋了，那我只能去寻找新的爱情了

感谢你曾经为我带来的一切
</blockquote>


### 2020.01.17

<blockquote>

当年的几个人，彭宇离开了南京，至今低调未曾露面；徐老太不堪周围辱骂，无奈搬家，于数年前死去，其子因违反规定被撤职；法官王浩受到此案影响，由堂堂法官沦为极为偏僻的办事处里无人问津的小公务员。

后续。“有人称之为“中国道德水平退步五十年”的开端

...

王浩被下放到司法所去了，再也不能干法官了。

其实这个事情当年开始的时候网络还没有这么发达，也就是王浩脑残非要弄得轰轰烈烈的。

说句不好听的话，王浩你非要判彭宇赔钱是没有关系，但是你要有水平啊，上来一句不是你撞得，你干嘛要垫付医药费？把自己给搞死了。

...

这个事件发生之前，我爹妈都是小声嘀咕告诉我：路上有老人倒了千万别扶啊，我们家可没有矿。

他们也知道，有些事可以做但是不能说，政治不正确。


这个事件发生后：我爹妈终于可以挺起腰杆理直气壮地告诉我不要扶了。不但要告诉我，还要和广大亲友互相通气，告知所有熟人碰到这种事千万不能扶。

...

这个王二所在的世界的审美观与其他世界都不太一样，按说其他世界中，一般都认为身材匀称、五官端正是好的，像王二这种大老爷们身高 160 公分、体重重大 163 斤，就显得又矮又肥胖，

...

我跟一位爱吃的长辈聊过这个，结论是：

——吃贵菜喝贵酒，若非为了社交，其实更多满足的是个好奇心，“到底是个嘛玩意？”

——相当多贵菜不一定是最好吃，更是食材稀缺、处理方法刁钻、工艺精湛。但那是艺术品范畴。

——许多好吃的食材所以便宜，是因为本身好吃，所以人类才大量培育。不好吃的东西，人类才不会去养呢。

——即，某种程度上，我们吃惯的，是祖先花了千年时间，证明这玩意好吃、好养活、好调理的东西啊。

...

那时候，我已经或多或少地，知道了世界有多大，也知道世界其实不太需要我们去拯救。

世上许多事，确实是稍微咬咬牙就能过去的；但也有许多事，咬了牙，并不一定过得去——生活比游戏，终究复杂得多。

有些什么流逝得飞快，而且并不由我决定。


但那个落雪午后，我确实觉得，自己似乎暂时回到了一个氛围里：

不管多么困苦艰难，只要兄弟齐心合力，咬咬牙，就可以拯救世界，然后，吃香喝辣，踌躇满志。

这种，我们以前确实相信过，多年后，依然希望其长存的心情。

...

いただきます　ごちそうさま

...

可能很多人会说，既然你这么想让我们关注炉石本身，那你为什么还要一而再再而三的去提到工资待遇这个问题，说到底你还不是想多挣钱？

是啊，我想多挣钱，一年前，大学未毕业，正值18岁青涩懵懂的年纪，愿意为了梦想为了爱好付出一切，包括青春。经过这一年洗礼，成长为一个24岁有担当的奔三的青壮年，该成家立业了。

我想当家人朋友亦或自己如果有一天生病踏进医院的时候有底气用最好的治疗手段，不用为钱发愁。

我想当家人朋友女朋友走进一个店的时候有底气去掏出钱包，不用担心价格，而不仅仅是过过眼瘾。

这是我认为我作为一个男人该做的，我该承担的责任。

人生百年，世间百态，众生牛马，寂寞如雪，不想功成名就名扬天下，只想在当地，做一个自由的较为英俊的，有底气的，有钱人。

...

“你快接句话 不然我感觉自己是老色批”
</blockquote>


### 2020.01.16

<blockquote>

看到一个校友说，

“北大那个事情（南方周末的报道）通篇读下来觉得匪夷所思又过于真实，尤其穿插校学生会选举十佳分票之类他人读起来不相关的事件，

在本校学生看来是人物形象跃然纸上，倒不是说这样的事情在北大发生就有什么特殊性，是这个校园的确太多垃圾事了，坐在高高的谷堆旁边我能讲它三天三夜”。

我很赞同ta的说法，这段话也提醒了我，宣传片里所谓“一派祥和”的北大校园或者其他高校校园里，其实大家压力都很大，会不会有更多压抑的故事潜伏着，

若没有争取引导会不会有更多悲剧，我们对于这样的情况又应该做些什么。

...

我前两天感冒刚好，鼻子里还正呼噜呼噜地流着青黄鼻涕，

最后我气得想笑憋得实在忍不住了，

又紧咬着牙关，

那口气就全从两个鼻孔里放出来了，

一只鼻孔以超高速喷射了一注青黄鼻涕，差点溅对面那厮身上，

一只鼻孔鼓了一个超大的鼻涕泡，差点盖住我半张脸。


对面那厮被我吓得哑口无言，良久才反应过来，

一边抬腿就跑，

一边嗷嗷叫说：“这他妈的是什么战术啊啊啊啊好他妈恶心啊啊啊啊”

...

那晚恰完饭、喝完酒出来，王二准备蹭他们车回去。

等代驾期间，王二的直属上级吴百科觉得仨大老爷们儿就那么叉着手傻站一块儿喝西北风面面相觑也太不像话，于是主动聊起酒这玩意儿。

王二最开始其实在梦游，看着他，却想着各种乱七八糟，想着赶紧回去打CP、回去勤学苦练，想着这回难得连晓东都来了，K这龟儿子居然那么调皮，找借口不来，想着那个憨批真的伤人心...

于是也没认真听，只晓得吴百科先是在说酒这东西成分、什么不同的酒，再说到什么适量饮酒有益、舒张心血管什么的，说着说着说起酒不好的一面，说少量的酒就可能对人体有害，甚至举例说：“...我的老婆weiai...”

？？？

听到这，王二一个哆嗦从梦里吓醒，严重怀疑是不是自己耳朵没有听清楚，便问他刚才说他老婆怎么了。

没想到吴百科一脸淡定地复述了前面的话，说是早期，还说起之前国庆那段时间不是请了长假吗，当时就是陪着自己老婆动手术去了，年后等下三个月了还得去复查...

王二听着感到有点不好意思，正想说些关切慰问的话，还没来得及，更让王二没想到的是，旁边王二的老大哥发话了，也一脸淡定地说起自己妈同样是早期胃癌动的手术...

王二当时就想，原来大家都挺不容易的。
</blockquote>


### 2020.01.15

<blockquote>

这是全球首例自杀式验毒，一名吸毒人员硬逼着法院给他验毒，最后成为了记录在册的涉毒分子。

...

当时看到的时候还蛮激动的，想上去合影，又觉得打扰人家不合适，就忍不住自己偷偷拍一张（虽然也不大好），结果还被姜文发现了。

姜文用那性感的京腔说，“长得挺好一小伙子，做事儿干嘛偷偷摸摸啊，想合照就大大方方的。”

然后下了飞机后，他稍微等了一下我，两人合了一张影，也算是挺有趣的经历。

...

跟女朋友吵架，你一定要认错，要无条件哄她，让着她。这是我认为三观最不正的话。

不知道哪个渣男总结的。

男女朋友间，是要在相互尊重的基础上沟通与交流的，一方一直哄着另一方，只会让对方的脾气越来越大，让对方越来越不讲道理，而且自己心理持续处于难受的状态。

长此以往，你心里难受，而对方的脾气被你惯坏了，对双方都没利益。

而且，遇到问题不好好沟通，一味的让着，只会让问题一直憋在心理，等哪天就会爆发出来，然后一发不可收拾，想想看，你跟你将来一起起床的人，连沟通都没有，炸弹就在心头里不知道什么时候就爆发了，你能过得下去吗？

当然了，这句话对渣男来说是很实用的。

毕竟他跟女生处一段时间就踹了，只馋身子，根本没打算长久一起生活，哄完拉倒，骗完就跑，毕竟他只忍一段时间，，甜言蜜语之后达成目的就走了，不可能长久度日。

哄完之后，他哄的对象脾气大了人难以与下一任相处了，他拍屁股走了，

...

正义或许会迟到，但永远不会缺席。

原句是：Justice delayed is justice denied.(迟到的正义绝非正义。)

...

“各位，假设你面对的是你的领导，你还会这么说话吗？”
</blockquote>


### 2020.01.14

<blockquote>

人的性格，往往是自己的经历造成的。绝大多数人的性格，都是一个套餐，没法单点。

性格活泼的人容易粗疏。性格沉静的人不免消极。有讨好倾向的人容易偏执。爱读书的人也容易认死理。

...

钱钟书先生《围城》里，方鸿渐去三闾大学教书前，也还有过美好想象；真到了那里，方知即便是草创的大学，也还是派系倾轧、勾心斗角，一片乱七八糟，着实是个是非窝。

读书人做起缺德事来，尤其容易让人心灰。因为大家多少存着点心思，“追名逐利的都是俗人，读书人好歹做事格调高些”；所以真遭遇了类似处境，真有些斯文扫地之感。

...

《天龙八部》里，萧峰感慨过这问题：

“为什么大家好好的都是人，却要强分为契丹、大宋？女真、高丽？你骂我辽狗？我骂你宋猪？”

...

つまらない

...

许多人会说“传统一路下来，一定有道理”。

然而许多所谓传统，最初只是想当然耳。

一路编排下来，越编越玄。了解风俗史的诸位都知道，许多传统民俗，都是如此从无到有，日益琐碎。

旧规矩不肯删除，新规矩越来越多，最后老的不肯改，少的必须依从，还编出一堆理由来撑着的。

男女关系上，许多禁忌，也是这么搞出来的。

...

用我某个编辑的话，她花重金买了某某色号的口红，结果一个月下来也就被两个塑料姐妹花同事问了，她男朋友更完全没领会到，颇让她有俏媚眼做给瞎子看了的明珠暗投之感。
</blockquote>


### 2020.01.13

<blockquote>

那几天王二那个监工兼八十岁的老母亲胡扒皮跑他那进行年底工作视察。见王二总的干得还算令她满意，便想扯些家常慰问一下。这不，那天又讲起王二那个关系有点八竿子打不着、之前小小年纪搞同性恋把新闻弄挺大的远房表妹，说什么现在才读初三，又谈了个男朋友搞得全校人尽皆知，被广播公开点名批评，还被拉校长办公室约谈，说什么那家的大人觉得自己这些年心血花了那么多，感觉不值，闹得个鸡飞狗跳。按说这么远的亲戚家的这些破事关王二鸟事，要是往常，一向沉默寡言的王二肯定不响，随胡扒皮扯她的淡。可这阵子王二刚好诸事不顺，心情抑郁，便借着这由头突然情绪发作，破口大骂到:“都真T娘的贪得无厌！我记得那家子父母上次还说什么只要她不做同性恋啥都依她，现在好了，变异性恋了，这不挺好的，不去好好支持，还想得寸进尺，限定什么上大学前不准谈朋友，做梦！”

...

也许他们各自事业有成，平时待人接物彬彬有礼，情商一流，但只要一扯到亲密关系这事上，说出来的话很像一个爱做梦的孩子。常见情况是女孩怕自己主动，男孩怕被拒绝。

...

你说你们每天扯着我问我怎么找到对的人谈恋爱，我让你去聊个天你说不好意思，我让你去多参加一点活动你说懒得动弹......

我又不是月老，总不能你天天在家里一坐，我直接给你快递过去一个皮囊和灵魂都五星好评的女朋友吧？

...

大概我妈的逻辑是，“人得会照顾自己且照顾别人，别人才会肯来找你。”很传统的想法。

我爸的逻辑是，“人会为了自己喜欢的人，自觉自愿地变好。”这个被我妈认为是臭美，但好像，更积极主动一点。

...

我知道总有人会说自己不愿意将就，但事实上将就不将就完全来源于你自己。

我之前问过一个女生，你心目中对的人应该是怎么样的？

女生回答：有钱、好看、聪明、有责任感、浪漫。

介于之前提到几乎匹配不到一百分的男人，那现在我们必须去掉一项，事实上八十分也已经算是很高分了。

女生去掉了浪漫。那么假设在恋爱结婚以后，对方就是很木讷一点都不浪漫，逢年过节什么礼物都没有一句情话都不会讲，对此你很不满意，那么请问这个时候你会不会觉得是在将就。

明白了么？将就这个事情永远是取决于你自身的心理状态，以前看重的事情以后未必看重，以前没想到的事情也有可能耿耿于怀。

每天都有那么多人离婚，难道他们结婚时候都不是真心实意？

但换言之哪怕一开始将就在一起，但在相处过程中彼此迁就互相理解，将就也能变成不将就。

心态决定了你在亲密关系中能否幸福，心态的差和谁在一起都是将就。这是我第三点要说的。

也有人问过我，在择偶的指标中，主次顺序应该怎么排。

我说先看内在核心，再看内在框架，剩下外在条件自由排序。

所谓的内心核心就是这个人的调性，基本的三观认知是否成熟，有没有完整独立的人格。

这是择偶的大前提，能达到这点的人起步60分。

还是和风险把控有关，和他们在一起，起码能保证他不犯大错：不会赌博，不会出轨，不会家暴，不会索取不付出……而且往往是潜力股。
</blockquote>


### 2020.01.09

<blockquote>

而且我顺便吐槽下微博上疯转的某些语录，比如，那个对的人啊，是你想捻也捻不掉揍也揍不跑的人，那些真爱啊，是你随便怎么样都会不离不弃的存在

——你知道这些“真爱”语录抓住了人的什么观念么？

好逸恶劳的观念。

培养了一个个公主病，国王病的青年，好像一个哪怕没有独立的经济能力和人格，哪怕性格在差，哪怕欲望在强也不懂控制的人，只要有真爱这个魔法，一切都解决啦。

你们不喜欢我，不是我性格有问题，不是我需要努力，不是我要变的更好，而是……你们不够真爱。

...

因为男人喜欢挑战，就说他们喜欢战斗和上战场，因此，应该尽量使他们无法征服你。这种说法就像是说女人喜欢洗厕所和刷地板、女人当二等公民是生活的自然秩序一样，真是可笑至极。

...

坊间劝酒常说，脸红的人不容易醉。是的，因为他们喝不了多少，相对于醉，他们更容易死。脸红，心跳加快都是饮酒后乙醛中毒的症状。

劝君更尽一杯酒，到了西天无故人。
</blockquote>


### 2020.01.07

<blockquote>

王小琴一到店，所有微商的人便都看着他笑。

有的叫道，“王小琴，你又把员工踢出微信群了！”

她不回答，对柜里说，“一份小年图，不要卡通风格的。”

便排出九文大钱。他们又故意的高声嚷道，“你一定是又强迫设计师加班作图了！”

王小琴睁大眼睛说，“你怎么这样凭空污人清白……”

“什么清白？我前天亲眼网上见你在群里要求设计师初一至初八每天做100张图，不做还要起诉人家。”

王小琴便涨红了脸，额上的青筋条条绽出，争辩道，“设计师加班不算加班……是正常工作安排！……上班时间每一分钟都要用于工作，……微商的事，能算强迫么？”

接连便是难懂的话，什么“政府高管”，什么“警车开道”，什么“国家政要，女王”之类，引得众人都哄笑起来。

店内外充满了快活的空气。

...

想起了我妈。

我妈：「说话啊，你哑巴了?」

我：「我没有哑巴。」

我妈：「哎呀，还敢顶嘴是吧?」

... 孩子他妈：“说话啊，你哑巴了?” 孩子：“我没有哑巴。” 孩子他妈：“哎呀，还敢顶嘴是吧?”

经历也好，知识也罢，察觉到自己匮乏，就会感到空虚，都会有欲望想去填满。

...

昨晚梦里像武打片一样，当时用着方言骂人打架，想想真T娘的巨（过）爽（瘾）

...

比起你们家有高中生女儿，我们读研快毕业的独生女儿，会更快面临这些问题，更需要父母担心操心。

比起从前，老婆现在似乎越来越豁达了。女儿小时候，她说希望女儿在身边；后来女儿上大学时，她说希望女儿回到省会，离家不远；现在似乎也在思考，如果工作事业和家庭有更好的选择，离家几百公里一两千公里的大城市，似乎也不应该阻拦。

...

印象里小时候好多人都对王二迷之友好，虽然现在也是，但以前太多人没能珍惜、没能久伴，没有机会说声感谢

...

王二所在的这个时代已经实现
</blockquote>


### 2020.01.05

<blockquote>

那天胡扒皮本是指导王二让他自己炒菜，结果炒的时候看王二太不像样，便训道：“哪有这么铲的！走过，我来”
</blockquote>


### 2020.01.03

<blockquote>

一场赌博引发的血案，王二的越南老婆成了盒，王家绝了后
</blockquote>


### 2020.01.02

<blockquote>

“没啥比看别人上班更有意思了！”

...

How To Be A Mom in 2017:

Make sure your children's academic, emotional, psychological, mental, spiritual, physical, nutritional, and social needs are met while being careful not to overstimulate, understimulate, improperly medicate, helicopter, or neglect them in a screen-free, processed foods-free, GMO-free, negative energy-free, plastic-free, body positive, socially conscious, egalitarian but also authoritative, nurturing but fostering of independence, gentle but not overly permissive, pesticide-free two-story, multilingual home preferably in a cul-de-sac with a backyard and 1.5 siblings spaced at least two year apart for proper development also don't forget the coconut oil.How To Be A Mom In Literally Every Generation Before Ours: Feed them sometimes.

翻译：

在2017年如何当个好家长？

你要确保你的孩子学术、情绪、心理、灵魂、身体、营养、和社交的需求都得以满足，同时你还要确保自己足够小心，不要过度操控孩子，也不要忽视他们；

不要错误用药；不要变成直升机式家长；不要给他们看过多的电子屏幕，不要给他们吃过度处理和转基因的食品；远离负能量，远离塑化剂；

对身体要有正面态度，对社交有足够的谨慎度；平等同时又要保持权威；给他们足够的滋养同时要保持他们的独立；温和但不要过度容让；

最好在家里讲N种语言，最好住在cul-de-sac（这个很难翻，指的是老美住房规划的一种，是住宅区内的死胡同形状，门前有个几家人共用的区间，很少有车出入，被认为是养娃最佳户型），

有后院，养2-3个孩子使他们得到手足关爱，并且孩子年龄间隔至少两岁从而使他们得到充分发展，同时也别忘了使用椰子油。

...

在我们之前的年代如何当个好家长？别饿死崽。

...

名场面：

“这个女孩唱滴不错。”

...

“之前有跟高中同学聊过一次天，寒暄之中，他就说了一句:‘真羡慕你现在过的神仙般的生活。’

一开始我会误解，他觉得我在当歌手或者在演艺圈里面，这是一种神仙般的生活，我其实有点不开心，以为每个人都会那样想，觉得大家不理解，不知道我有多辛苦，只知道我们光鲜的那一面。

后来跟他聊下去之后发现，他说的那个神仙般的生活，说的是我做的工作是自己喜欢的事情。

他是男生，慢慢感觉自己已经变成了老男孩，但我还在追梦的路上。

那一刻我心里还挺震撼的，所以我觉得我很幸运，真的很幸福。

我也希望现在还年轻的朋友们，能找到自己喜欢的一件事情，很重要很重要。如果每天都在做着无聊、不喜欢的事，会很不开心。

但如果你每天都在做着自己喜欢的事情，哪怕每天不停地重复它们，就像我唱《大鱼》很多遍，现在每次唱都还会很开心，因为我觉得是这首歌让很多人认识到了我。”
</blockquote>
