

一、粗饼后台需求功能增加

1. 功能增加表

     <table> 
               <tr style="white-space: nowrap;">
                   <th>一级栏目</th>
                   <th>二级栏目</th>
                   <th>页面链接</th>
                   <th>需求</th>
                   <th>次需求</th>
               </tr>
               <tr>
                  <td rowspan="3">比赛</td>
                  <td>比赛管理</td>
                  <td><a href="https://staging.cubingchina.com/board">页面链接</a></td>
                  <td>
                   比赛管理状态更改 >> <br>
                   1. 初审通过（申请页面点击初审通过）；<br>
                   2. 代表已分配（编辑页面增加分配代表功能）；<br>
                   3. 复审通过（编辑页面增加复审通过） ；<br>
                   4. 待公示（复审通过后为此状态）；<br>
                   5. 锁定（只能操作锁定日期31天以上的比赛）；<br>
                   6. 已公示；<br>
                  </td>
                  <td>---</td>
               </tr>
               <tr>
                   <td>申请比赛</td>
                   <td><a href="https://staging.cubingchina.com/board/competition/apply">页面链接</a></td>
                   <td>
                       1. 只能选择填表日期60天以上的日期（WCA）；<br>
                       2. 隐藏选择代表的选项；（初审不需要填写代表）；<br>
                       3. 通知给competitions@cubing.com；<br>
                       4. 查询经纬度坐标网站进不去；<br>
                       5. 操作页面的 通过 改为 初审通过（之后的状态随比赛管理状态同步）；<br>
                       6. 增加“隐藏公告”按钮功能（需和新闻列表状态同步）；<br>
                       7. 增加WCA新人月比赛开关按钮；<br>
                       8. 增加WCA系列赛链接和前台详情页面显示；<br>
                   </td>
                   <td>
                       1.审核期（回复）为7个自然日，设置临期3天、1天提醒警告；<br>
                       2.增加tab(提交比赛策划案，限制pdf格式，文件个数限制5个) 基本信息隐提交按钮<br>
                       审核组增加查看，驳回/拒绝按钮。查看最新一次驳回原因。通过信息展示，提交策划案tab隐藏；
                   </td>
               </tr>
               <tr>
                   <td>申请列表</td>
                   <td><a href="https://staging.cubingchina.com/board/competition/application">页面链接</a></td>
                   <td>
                       1. 点击比赛操作，可查看比赛拒绝原因/历史驳回原因和时间点；
                   </td>
                   <td>
                     ----
                   </td>
               </tr>
               <tr>
                   <td>用户</td>
                   <td>数据统计</td>
                   <td><a href="https://staging.cubingchina.com/board/user/statistics">页面链接</a></td>
                   <td>
                       ---
                   </td>
                   <td>
                       1. 增加每个季度比赛数量echats图表数据分析（确认、拒绝比赛数量）；
                   </td>
               </tr>
               <tr>
                   <td>配置</td>
                   <td>权限配置（新增）</td>
                   <td><a href="https://staging.cubingchina.com/board">页面链接</a></td>
                   <td>
                       1.根据账号，修改为checkbox多选自定义权限，赋予账号对应权限（权限表在下方）；
                   </td>
                   <td>
                       ---
                   </td>
               </tr>
               <tr>
                   <td rowspan="2">新闻</td>
                   <td>新闻管理</td>
                   <td><a href="https://staging.cubingchina.com/board/news/index">页面链接</a></td>
                   <td>
                       1. 新闻列表状态 需和 申请比赛 操作状态对应（联动关系）；<br> 
                       2. 新闻关键词搜索；
                   </td>
                   <td>
                       1.前台搜索页面；
                   </td>
               </tr>
               <tr>
                   <td>新增新闻</td>
                   <td><a href="https://staging.cubingchina.com/board/news/add">页面链接</a></td>
                   <td>
                       1. 增加新闻公告“预览”按钮。需弹框展示；
                   </td>
                   <td>
                       ---
                   </td>
               </tr>
               <tr>
                   <td>FAQ</td>
                   <td>新增FAQ</td>
                   <td><a href="https://staging.cubingchina.com/board/faq/add">页面链接</a></td>
                   <td>
                       1. 增加FAQ“预览”按钮。需弹框展示；
                   </td>
                   <td>
                       ---
                   </td>
               </tr>
       </table>



二、粗饼账号权限分配表

| 粗饼账号权限分配表                                           |               |        |                                                   |            |                                      |                                             |                    |                     |
| ------------------------------------------------------------ | :------------ | ------ | ------------------------------------------------- | ---------- | ------------------------------------ | ------------------------------------------- | ------------------ | ------------------- |
| 名称/项目                                                    | 英文          | 管理员 | WCA代表                                           | 用户管理组 | 粗饼赛事审核与质量保证组（公共账号） | 粗饼赛事审核与质量保证组（WCA比赛管理成员） | 通讯组（粗饼/WCT） | 主办方              |
| 比赛                                                         | Competitions  |        |                                                   |            |                                      |                                             |                    |                     |
| 比赛管理                                                     | manage        | √      | √（针对自己监督比赛，其他代表仅查看不能编辑权限） |            | √                                    | √                                           |                    | √（针对自己的比赛） |
| 申请比赛                                                     | applu         | √      | √                                                 |            | √                                    | √                                           |                    | √                   |
| 申请列表                                                     | list          | √      | √（针对自己监督比赛，其他代表仅查看不能编辑权限） |            | √                                    | √                                           |                    | √（针对自己的比赛） |
| 报名                                                         | Registration  |        |                                                   |            |                                      |                                             |                    |                     |
| 报名管理                                                     | admin         | √      | √（针对自己监督比赛）                             |            | √                                    |                                             |                    | √（针对自己的比赛） |
| 用户                                                         | Users         |        |                                                   |            |                                      |                                             |                    |                     |
| 用户管理                                                     | admin         | √      | √                                                 | √          | √                                    |                                             |                    |                     |
| 重复用户                                                     | repeat        | √      | √                                                 | √          | √                                    |                                             |                    |                     |
| 合并用户                                                     | merge         | √      | √                                                 | √          | √                                    |                                             |                    |                     |
| 数据统计                                                     | statistics    | √      | √                                                 | √          | √                                    |                                             | √                  | √                   |
| 群发邮件                                                     | bulk          | √      |                                                   | √          |                                      |                                             | √                  |                     |
| 财务                                                         | Pay           |        |                                                   |            |                                      |                                             |                    |                     |
| 支付流水                                                     | payment flow  | √      | √                                                 |            | √                                    |                                             |                    | √（针对自己的比赛） |
| 对账单                                                       | statement     | √      |                                                   |            |                                      |                                             |                    |                     |
| 新闻                                                         | News          |        |                                                   |            |                                      |                                             |                    |                     |
| 新闻管理                                                     | admin         | √      | √                                                 |            | √                                    |                                             | √                  |                     |
| 发布新闻                                                     | release       | √      | √                                                 |            | √                                    |                                             | √                  |                     |
| 新闻模板                                                     | template      | √      |                                                   |            |                                      |                                             |                    |                     |
| 配置                                                         | Configuration |        |                                                   |            |                                      |                                             |                    |                     |
| 配置管理                                                     | admin         | √      |                                                   |            |                                      |                                             |                    |                     |
| 配置权限（新增）                                             | permission    | √      |                                                   |            |                                      |                                             |                    |                     |
| 总结                                                         | Conclusion    |        |                                                   |            |                                      |                                             |                    |                     |
| 评价管理                                                     | admin         | √      | √                                                 |            | √                                    |                                             |                    |                     |
| 主办总结                                                     | summarize     | √      |                                                   |            | √                                    |                                             |                    | √                   |
| 代表评价                                                     | evaluation    | √      |                                                   |            | √                                    |                                             |                    |                     |
| FAQ                                                          | FAQ           |        |                                                   |            |                                      |                                             |                    |                     |
| FAQ管理                                                      | admin         | √      |                                                   |            | √                                    |                                             | √                  |                     |
| 新增FAQ                                                      | add           | √      |                                                   |            | √                                    |                                             | √                  |                     |
| FAQ分类                                                      | type          | √      |                                                   |            | √                                    |                                             | √                  |                     |
| 备注：根据账号，修改为checkbox多选自定义权限，赋予账号对应权限 |               |        |                                                   |            |                                      |                                             |                    |                     |