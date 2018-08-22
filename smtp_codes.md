
#### 摘自：http://cn.evo-mailserver.com.tw/support/smtp_error_code.php

<table>
    <caption>
    错误总表
    </caption>
    <tr>
        <td width="60" rowspan="2">420</td>
        <td width="480">1. Timeout Communication Problem Encountered During Transmission.  Thie Is a Novell Groupwise Smtp Error 2. Tcp Read Error 3. Tcp Write Error</td>
        <td width="400" class="desc">在联机时发生通讯中断的问题；Novell GroupWise SMTP服务器的错误讯息</td>
    </tr>
    <tr>
        <td>此错误讯息只适用于Novell GroupWise SMTP服务器，在此不多做赘述。</td>
        <td class="desc">N/A</td>
    </tr>
    <tr>
        <td rowspan="2">421</td>
        <td>1. <domain> Service Not Available, Closing  Transmission Channel [this May Be a Reply To Any Command If the Service Knows It Must Shut Down] 2. <server name=""> Service Not Available - the Sending Email Program Should Try Again Later</server></domain></td>
        <td class="desc">括号内的主机无法提供正常的邮件服务，关闭传送管道，邮件将滞留在主机上</td>
    </tr>
    <tr>
        <td>收信者端邮件服务器暂时无法上线。</td>
        <td class="desc">请收信者和邮件管理者确认收信端邮件服务器是否正常作业，通常是由于邮递员停机做问题的检测或是邮件服务器正在重开机中又或是服务器正在同时间处理大量的新进邮件或新进要求。这类情形不会持续太久，若能晚点在尝试发送，也许问题已经解决。请注意的是：这里指的邮件服务器可能是邮件发送途中的任何一台邮件服务器。若是这种情形发生的太过于频繁，则需要与邮递员讨论。</td>
    </tr>
    <tr>
        <td rowspan="2">421</td>
        <td>1. the Smtp Service/server You Use Has a Limit On the Number of Concurrent Smtp Streams Your Server Can Use
    2. Too Many Concurrent Smtp Connections From This Ip Address; Please Try Again Later</td>
        <td class="desc">收件者 SMTP 主机拒绝提供服务，因为已经超过其能提供的最大服务量</td>
    </tr>
    <tr>
        <td>SMTP 主机最大联机数量已达</td>
        <td class="desc">稍后再试</td>
    </tr>
    <tr>
        <td rowspan="2">422</td>
        <td>The Recipient's Mailbox Is Over Its Storage Limit</td>
        <td class="desc">收信者邮件信箱的信件已经超过允许的最大容量</td>
    </tr>
    <tr>
        <td>可能收信者信箱被塞满</td>
        <td class="desc">1. 请收信者整理邮件信箱
    2. 请收信者通知邮递员加大信箱空间</td>
    </tr>
    <tr>
        <td rowspan="2">422</td>
        <td>The Size of the Message Exceeds the Recipient's Size Limits For Incoming Emails</td>
        <td class="desc">邮件大小超过收信端邮件信箱的单次收信大小</td>
    </tr>
    <tr>
        <td>邮件大小超过收信端邮件信箱的单次收信大小。</td>
        <td class="desc">1. 请收信者通知邮递员加大单次收信大小；
    2. 收信者通知发件人分次寄送过大信件的内容。</td>
    </tr>
    <tr>
        <td rowspan="2">431</td>
        <td>The Recipient's Mail Server Is Experiencing a Disk Full Condition</td>
        <td class="desc">收信端的邮件服务器磁盘空间已满</td>
    </tr>
    <tr>
        <td>收信端的邮件服务器磁盘空间已满</td>
        <td class="desc">请收信者通知邮递员清出可用空间以供使用</td>
    </tr>
    <tr>
        <td rowspan="2">432</td>
        <td>The Recipient's Exchange Server Incoming Mail Queue Has Been Stopped</td>
        <td class="desc">收信者的 Exchange Server 的新进信件处理程序已经停止</td>
    </tr>
    <tr>
        <td>通常是Exchange Server 管理者正在处理一些问题。</td>
        <td class="desc">请收信者通知邮递员处理。</td>
    </tr>
    <tr>
        <td rowspan="2">441</td>
        <td>The Recipient's Server Is Not Responding</td>
        <td class="desc">收信端的邮件服务器没有回应</td>
    </tr>
    <tr>
        <td>收件端邮件服务器没有反应，可能正在维护中</td>
        <td class="desc">寄信端邮件服务器会再次或多次尝试寄送，您无需担心</td>
    </tr>
    <tr>
        <td rowspan="2">442</td>
        <td>The Connection Was Dropped During Transmission</td>
        <td class="desc">传送邮件的过程中联机中断</td>
    </tr>
    <tr>
        <td>传送的过程中联机中断</td>
        <td class="desc">1. 检查邮件是否带有病毒附件
    2. 当然病毒或是黑客的可能性也不容忽视。</td>
    </tr>
    <tr>
        <td rowspan="2">446</td>
        <td>The Maximum Hop Count Was Exceeded For the Message</td>
        <td class="desc">邮件传送时经过的服务器跃点数已经超过最大值</td>
    </tr>
    <tr>
        <td>邮件可能在内部网络中的两台服务器中被转来转去以致于超过最大跃点数；也有可能是邮件在发信端与收信端的邮件服务器之间来回跳跃，而造成超过最大跃点数</td>
        <td class="desc">请与ISP联络检查网络问题</td>
    </tr>
    <tr>
        <td rowspan="2">449</td>
        <td>Routing Error</td>
        <td class="desc">路由错误</td>
    </tr>
    <tr>
        <td>此错误讯息只适用于Microsoft Exchange Server，在此不多做赘述。</td>
        <td class="desc">通知收件者网络管理员</td>
    </tr>
    <tr>
        <td rowspan="2">450</td>
        <td>Requested Mail Action Not Taken -  the Mailbox Was Unavailable at the Remote End</td>
        <td class="desc">所要求的邮件动作无法执行：收信端无此账户</td>
    </tr>
    <tr>
        <td>收信端无此账户</td>
        <td class="desc">检查是否拼错字</td>
    </tr>
    <tr>
        <td rowspan="2">450</td>
        <td>Please Try Again Later</td>
        <td class="desc">请在尝试一次</td>
    </tr>
    <tr>
        <td>通常发生在对方启用灰名单防垃圾信机制的缘故</td>
        <td class="desc">无需理会，让服务器自动重寄</td>
    </tr>
    <tr>
        <td rowspan="2">450</td>
        <td>Host Down</td>
        <td class="desc">邮件服务器不在在线</td>
    </tr>
    <tr>
        <td>收信端邮件主机故障</td>
        <td class="desc">稍后再重寄</td>
    </tr>
    <tr>
        <td rowspan="2">450 5.2.3</td>
        <td>Msg Size Greater Than Allowed By Remote Host</td>
        <td class="desc">邮件大小超过收信端的上限</td>
    </tr>
    <tr>
        <td>邮件大小超过收信端的上限</td>
        <td class="desc">1. 请缩小单笔邮件的大小，可将一封邮件切为多封邮件来传送
    2. 请收信端邮递员将收信上限提高
    3. 若是还是无法寄送，可以考虑使用FTP的传输方式来传送</td>
    </tr>
    <tr>
        <td rowspan="2">451</td>
        <td>Requested Action Aborted: Local Error in Processing</td>
        <td class="desc">要求动作中断：在本地处理邮件时产生错误</td>
    </tr>
    <tr>
        <td>原因1：收信端 SMTP 软件可能已经当机</td>
        <td class="desc">请寄信者针对此问题通知对方网络管理员</td>
    </tr>
    <tr>
        <td rowspan="2">451</td>
        <td>(x.x.x.x) Has Recently Sent Spam</td>
        <td class="desc">(x.x.x.x) 被认定近期常发送垃圾信</td>
    </tr>
    <tr>
        <td>IP地址可能落在垃圾信IP数据库内</td>
        <td class="desc">请邮递员检验相关垃圾信来源的数据库</td>
    </tr>
    <tr>
        <td rowspan="2">451</td>
        <td>Requested Action Delayed – Local Problem</td>
        <td class="desc">传输延迟：指令被延迟，本地的错误</td>
    </tr>
    <tr>
        <td>此问题表示收件者邮件服务器故障</td>
        <td class="desc">稍后在试或通知收件者网络管理员</td>
    </tr>
    <tr>
        <td rowspan="2">451</td>
        <td>Unable To Complete Command, Dns Not Available Or Timed Out</td>
        <td class="desc">无法完成指令，DNS系统无法提供服务导致服务停摆</td>
    </tr>
    <tr>
        <td>DNS解析的问题</td>
        <td class="desc">收信端邮件服务器主机无法解析DNS，请稍后在试</td>
    </tr>
    <tr>
        <td rowspan="2">451</td>
        <td>Domain of Sender Address Does Not Resolve</td>
        <td class="desc">无法解析发信者的邮件地址</td>
    </tr>
    <tr>
        <td>DNS解析的问题</td>
        <td class="desc">请检查寄信端邮件服务器网络卡设定以及确认该DNS服务器是否正常工作;</td>
    </tr>
    <tr>
        <td rowspan="2">451</td>
        <td>Max Smtp Services Exceeded, Please Try Again Later</td>
        <td class="desc">已超过最高的SMTP联机数，请稍后再试</td>
    </tr>
    <tr>
        <td>SMTP服务太过繁忙；可能被当垃圾信跳板服务器。</td>
        <td class="desc">1. 提高最高SMTP联机数并且稍后再试
    2. 关闭 Open Relay 
    3. 开启 SMTP AUTH 身份认证</td>
    </tr>
    <tr>
        <td rowspan="2">451</td>
        <td>Read Error From Mail.mail.xxx.xxx.xxx</td>
        <td class="desc">读取错误自&lt;邮件服务器&gt;</td>
    </tr>
    <tr>
        <td>可能是DNS指向设定错误。</td>
        <td class="desc">1. 请检查DNS是否正常运作</td>
    </tr>
    <tr>
        <td rowspan="2">451 4.1.8</td>
        <td>Domain of Sender Address Xxx@xxx.xxx Does Not Resolve</td>
        <td class="desc">无法解析送信者邮件信箱所属的网域</td>
    </tr>
    <tr>
        <td>DNS的问题比如需要做DNS反解。</td>
        <td class="desc">通知邮递员并检查DNS设定是否正常。</td>
    </tr>
    <tr>
        <td rowspan="2">451 4.7.1</td>
        <td>Greylisting in Action, Please Come Back in 00:02:00 [minutes]</td>
        <td class="desc">灰色名单功能运行中，请在两分钟后再寄一次邮件</td>
    </tr>
    <tr>
        <td>灰色名单功能运行中</td>
        <td class="desc">请在两分钟后再寄一次邮件（服务器会自动重寄）</td>
    </tr>
    <tr>
        <td rowspan="2">452</td>
        <td>Requested Action Not Taken: Insufficient System Storage</td>
        <td class="desc">要求动作无法执行：系统空间不足</td>
    </tr>
    <tr>
        <td>收件者邮件服务器硬盘可能已满</td>
        <td class="desc">解决办法是等一段时间之后再行寄，或者通知收信者网络管理员</td>
    </tr>
    <tr>
        <td rowspan="2">452</td>
        <td>Too Many Recipients</td>
        <td class="desc">在单次待发邮件中有过多收信者邮件账号</td>
    </tr>
    <tr>
        <td>此问题可能发生在寄信端ISP、收信端ISP或甚至是发信端邮件服务器：由于一些其他的问题发生导致所有使用者无法发信件，当问题修复完成时的那一瞬间，所有的信件一下子蜂拥而至塞满服务器的储存空间甚至也塞满系统内存的资源，此错误讯息就会发生。</td>
        <td class="desc">1. 解决办法是等一段时间之后，等尖峰期过后再行寄送。</td>
    </tr>
    <tr>
        <td rowspan="2">452</td>
        <td>Out of Memory</td>
        <td class="desc">内存不足</td>
    </tr>
    <tr>
        <td>此问题可能发生在寄信端ISP、收信端ISP或甚至是发信端邮件服务器：由于一些其他的问题发生导致所有使用者无法发信件，当问题修复完成时的那一瞬间，所有的信件一下子蜂拥而至塞满服务器的储存空间甚至也塞满系统内存的资源，此错误讯息就会发生。</td>
        <td class="desc">1. 解决办法是等一段时间之后，等尖峰期过后再行寄送。</td>
    </tr>
    <tr>
        <td rowspan="2">465</td>
        <td>Invalid Response Code Received From Server</td>
        <td class="desc">自服务器接收到无效的认证回应</td>
    </tr>
    <tr>
        <td>自2010年开始，osTicket或是其他的邮件服务器开始使用此错误代码，若是认证设定有错误时，收信者的邮件服务器会回应此错误代码。</td>
        <td class="desc">1. 请收信者联络邮递员解决认证设定上的修正。</td>
    </tr>
    <tr>
        <td rowspan="2">471</td>
        <td>This Is a Local Error With the Sending Server And Is Often Followed With “please Try Again Later”</td>
        <td class="desc">发信端的邮件服务器自身发生错误时，时常会回报请稍候再试</td>
    </tr>
    <tr>
        <td>此错误码471或4.7.1经常被当作一般SMTP错误码的附带码比如：451 4.7.1。
    原因一：有此附带码的错误通常都和寄信端邮件服务器上的反垃圾信机制或是防病毒软件有关连。并且是由这类程序内的程序瑕疵或程序自动更新机制所造成。
    原因二：内存不足或硬盘上的数据损毁等等硬件上的问题。</td>
        <td class="desc">原因1：
    1. 与软件商联络咨询有无解法；
    2. 若这些软件并非专门的邮件服务器版本时，将邮件扫瞄的功能关闭。
    原因2：
    1. 与邮递员联系并做硬件除错。</td>
    </tr>
    <tr>
        <td rowspan="2">500</td>
        <td>Syntax Error, Command Not Recognized [this May Include Errors Such As Command Line Too Long]</td>
        <td class="desc">语法错误，无法辨识的指令</td>
    </tr>
    <tr>
        <td>原因：1. 最后一个从发信端邮件服务器发出的SMTP或ESMTP指令无法为收件者的服务器所辨识。
    原因2. 或是指令的格式不符合对方服务器的要求，此间包含指令字符串太长上述两个原因通常是防病毒软件或是防火墙程序对于SMTP进或出的端口造成影响。</td>
        <td class="desc">可能有防火墙软硬件阻挡了一些新型态的 SMTP 指令，可关闭防火墙或防病毒软件进行测试</td>
    </tr>
    <tr>
        <td rowspan="2">500</td>
        <td>Line Too Long</td>
        <td class="desc">指令太长，无法辨识</td>
    </tr>
    <tr>
        <td>指令的格式不符合对方服务器的要求，此间包含指令字符串太长。</td>
        <td class="desc">请参考防病毒软件或是防火墙程序的使用手册上和SMTP相关的对应设定。</td>
    </tr>
    <tr>
        <td rowspan="2">500</td>
        <td>Access Denied By Port Access</td>
        <td class="desc">端口存取被拒</td>
    </tr>
    <tr>
        <td>指令的格式不符合对方服务器的要求，此间包含指令字符串太长。</td>
        <td class="desc">请参考防病毒软件或是防火墙程序的使用手册上和SMTP相关的对应设定。</td>
    </tr>
    <tr>
        <td rowspan="2">500</td>
        <td>Unrecognized Command</td>
        <td class="desc">无法辨识的指令</td>
    </tr>
    <tr>
        <td>最后一个从发信端邮件服务器发出的SMTP或ESMTP指令无法为收件者的服务器所辨识。</td>
        <td class="desc">请参考防病毒软件或是防火墙程序的使用手册上和SMTP相关的对应设定。</td>
    </tr>
    <tr>
        <td rowspan="2">501</td>
        <td>Can Sometimes Also Be Indicative of Communication Problems</td>
        <td class="desc">有时可能是网络线路的问题</td>
    </tr>
    <tr>
        <td>网络线路的问题。</td>
        <td class="desc">请在command prompt底下键入ping 168.95.1.1还有ping其他响应快速的网站比如www.microsoft.com以及www.hinet.net等等来测试网络是否顺畅。若出现响应时间太慢或是有断讯的现象，请向网络管理员反映。</td>
    </tr>
    <tr>
        <td rowspan="2">501</td>
        <td>Sender Email Is Not in My Domain</td>
        <td class="desc">发信者账号不在发信者所属网域</td>
    </tr>
    <tr>
        <td>笔误</td>
        <td class="desc">请确认发件人账号无误</td>
    </tr>
    <tr>
        <td rowspan="2">501</td>
        <td>Recipient Is Not Verified</td>
        <td class="desc">无法确认收信者的邮件账号</td>
    </tr>
    <tr>
        <td>收信者的邮件账号可能输入错误。</td>
        <td class="desc">请与对方确认邮件账号。</td>
    </tr>
    <tr>
        <td rowspan="2">501</td>
        <td>Sender Domain Must Exist</td>
        <td class="desc">发信者的网域必须存在</td>
    </tr>
    <tr>
        <td>原因1：DNS的问题
    原因2：发件人邮件地址域名可能输入错误</td>
        <td class="desc">原因1： 请确认DNS设定没问题
    原因2： 请确认邮件账号中的域名是正确的</td>
    </tr>
    <tr>
        <td rowspan="2">501</td>
        <td>Syntax Error in Parameters Or Arguments</td>
        <td class="desc">系统指令的参数错误</td>
    </tr>
    <tr>
        <td>系统指令的参数错误</td>
        <td class="desc">1. 请确认.信箱账号无误
    2. 网域名无误
    3. Linux/Unix 的SEND MAIL 指令依照标准语法</td>
    </tr>
    <tr>
        <td rowspan="2">501</td>
        <td>Path Too Long</td>
        <td class="desc">系统指令的参数错误</td>
    </tr>
    <tr>
        <td>系统指令的参数错误。</td>
        <td class="desc">请确认指令参数符合标准</td>
    </tr>
    <tr>
        <td rowspan="2">501</td>
        <td>Syntax Helo Hostname</td>
        <td class="desc">语法: HELO hostname</td>
    </tr>
    <tr>
        <td>收信者邮件服务器要求发件人邮件服务器发送正确的指令语法</td>
        <td class="desc">使用 EVO Mail Server 应不致于有这款问题</td>
    </tr>
    <tr>
        <td rowspan="2">501</td>
        <td>Invalid Domain Name</td>
        <td class="desc">无效的域名</td>
    </tr>
    <tr>
        <td>无效的域名。</td>
        <td class="desc">请确认域名无误。</td>
    </tr>
    <tr>
        <td rowspan="2">501 5.1.3</td>
        <td>Invalid Address</td>
        <td class="desc">无效的邮件地址</td>
    </tr>
    <tr>
        <td>无效的邮件地址。</td>
        <td class="desc">请确认邮件地址无误。</td>
    </tr>
    <tr>
        <td rowspan="2">501 5.1.3</td>
        <td>Bad Recipient Address Syntax</td>
        <td class="desc">收信者邮件账号语法错误</td>
    </tr>
    <tr>
        <td>收信端邮件账号语法错误。</td>
        <td class="desc">请确认邮件地址无误。</td>
    </tr>
    <tr>
        <td rowspan="2">501 5.5.4</td>
        <td>Invalid Address</td>
        <td class="desc">不合法的IP地址</td>
    </tr>
    <tr>
        <td>若收信端邮件服务器是MS Exchange Server 5.5， 2000， 2003而收到此错误讯息时，</td>
        <td class="desc">请与收信端邮递员联络并附上http://support.microsoft.com/kb/291828.将Exchange Server予以修正。</td>
    </tr>
    <tr>
        <td rowspan="2">502</td>
        <td>1. Unimplemented Command
    2. Command Not Implemented</td>
        <td class="desc">SMTP指令的语法错误，原因不明</td>
    </tr>
    <tr>
        <td>收件者邮件服务器主机不支持某些基本的 SMTP 指令</td>
        <td class="desc">联系对方邮递员并建议它更新软件</td>
    </tr>
    <tr>
        <td rowspan="2">503</td>
        <td>1. Polite People Say Helo First
    2. Error: Need Mail Command
    3. Need Mail Before Rcpt
    4. Bad Sequence of Commands</td>
        <td class="desc">SMTP指令顺序出错，一般出现在其他错误之后，先检查之前出现的错误提示</td>
    </tr>
    <tr>
        <td>这类问题通常是寄件用 SMTP 软件设计不良或是防火墙造成</td>
        <td class="desc">替 SMTP 软件更新版本并检查防火墙是否有阻止某些指令</td>
    </tr>
    <tr>
        <td rowspan="2">503</td>
        <td>This Mail Server Requires Authentication When Attempting To Send To a Non-local E-mail Address. Please Check Your Mail Client Settings Or Contact Your Administrator To Verify That the Domain Or Address Is Defined For This Server</td>
        <td class="desc">邮件服务器需要身份认证，请检查收信软件中的设定</td>
    </tr>
    <tr>
        <td>寄信者若没有经过身份认证将无法对网域外的收信者发信</td>
        <td class="desc">请在Outlook里的「我的 SMTP 服务器需要验证」打勾来启动 SMTP Auth 的功能</td>
    </tr>
    <tr>
        <td rowspan="2">503</td>
        <td>No Recipients Specified</td>
        <td class="desc">没有指定收信者</td>
    </tr>
    <tr>
        <td>收信者字段若没有指定邮件账号，信件无法寄出</td>
        <td class="desc">请在收信者字段输入收信者电子邮件账号</td>
    </tr>
    <tr>
        <td rowspan="2">504</td>
        <td>1. Command Parameter Not Implemented
    2. Need To Authenticate First</td>
        <td class="desc">1. 此SMTP指令没有内建此参数 
    2. 登入之前需要认证</td>
    </tr>
    <tr>
        <td>在邮件服务器内，此指令无设此参数而造成验证失败</td>
        <td class="desc">请收信者洽邮递员</td>
    </tr>
    <tr>
        <td rowspan="2">505</td>
        <td>Client Was Not Authenticated</td>
        <td class="desc">客户端没有经过认证无法登入</td>
    </tr>
    <tr>
        <td>在Outlook或是Outlook Express里使用gmail或是yahoo信箱的Smtp服务器时，若没有设定好一些选项，会出现此项错误讯息。</td>
        <td class="desc">1. 要用雅虎或GMAIL的邮箱发信；
    2. 要加入身份验证；
    3. 要在「个人信息」中填写正确邮箱地址；
    4. 要点选「SMTP服务器需要认证」。</td>
    </tr>
    <tr>
        <td rowspan="2">510</td>
        <td>Bad Email Address</td>
        <td class="desc">无效的电子邮件账号</td>
    </tr>
    <tr>
        <td>此错误讯息发自寄信端邮件服务器。若是TO， CC， BCC的收信者位在网域内，表示这些收信者不存在；若是收信者是收信者邮件账号是网外账号，表示这些账号可能笔误。</td>
        <td class="desc">请确认收件端账号是否正确。</td>
    </tr>
    <tr>
        <td rowspan="2">511</td>
        <td>1. Bad Email Address
    2. Sorry, Recipient Address Has Invalid Format</td>
        <td class="desc">1. 无效的邮件账号
    2. 收件者信箱格式错误</td>
    </tr>
    <tr>
        <td>表示这些收件者电子邮件地址可能有笔误</td>
        <td class="desc">请确认收件端账号是否正确</td>
    </tr>
    <tr>
        <td rowspan="2">512</td>
        <td>The Host Server For the Recipient’s Domain Name Cannot Be Found (dns Error)</td>
        <td class="desc">找不到负责收信者邮件账号的邮件服务器主机</td>
    </tr>
    <tr>
        <td>若是一切都正确，则有可能是DNS服务器上的解析纪录有问题，通常是负责本身邮件服务器的DNS服务器或是所属ISP的DNS服务器无法正确解析。</td>
        <td class="desc">请逐一检查所有收信端邮件地址的网域名是否正确。</td>
    </tr>
    <tr>
        <td rowspan="2">512</td>
        <td>Bad Destination Host 'dns Hard Error Looking Up Domain</td>
        <td class="desc">DNS系统中找不到这收信者的网域名</td>
    </tr>
    <tr>
        <td>主要是DNS系统无法解析</td>
        <td class="desc">请逐一检查所有收信端邮件地址的网域名是否正确。</td>
    </tr>
    <tr>
        <td rowspan="2">512</td>
        <td>The Message Could Not Be Delivered Because the Recipient's Destination Email System Is Unknown Or Invalid. Please Check the Address And Try Again, Or Contact Your System Administrator To Verify Connectivity To the Email System of the Recipient</td>
        <td class="desc">收信者的邮件服务器或是邮件信箱账号可能出现问题以致于无法传递信件，请洽网络管理员以确认收信者的邮件系统是否正常</td>
    </tr>
    <tr>
        <td>若是一切都正确，则有可能是DNS服务器上的解析纪录有问题，通常是负责本身邮件服务器的DNS服务器或是所属ISP的DNS服务器无法正确解析。</td>
        <td class="desc">可通知邮递员加以确认。</td>
    </tr>
    <tr>
        <td rowspan="2">512</td>
        <td>Conditions are Caused By Misspellings of the Domain Name Part of a Recipient Email Address</td>
        <td class="desc">收信者邮件地指的网域部分可能有错误，以致于出现此问题</td>
    </tr>
    <tr>
        <td>主要是DNS系统无法解析邮件里TO，CC，BCC中信箱地址的网域名。</td>
        <td class="desc">请逐一检查所有收信端邮件地址的网域名是否正确。</td>
    </tr>
    <tr>
        <td rowspan="2">513</td>
        <td>Relaying Denied Or Authentication Required (a Small Percentage of Mail Servers)</td>
        <td class="desc">邮件寄送被拒或是需要验证（一小部分的邮件服务器有此规范）</td>
    </tr>
    <tr>
        <td>小部分的邮件服务器需要寄信者在寄信之前做身份的验证。</td>
        <td class="desc">请邮件服务器管理员确认认证步骤并在邮件程序里设定好安全验证的步骤</td>
    </tr>
    <tr>
        <td rowspan="2">523</td>
        <td>The Recipient’s Mailbox Cannot Receive Messages This Big</td>
        <td class="desc">由于信箱大小的上限，收信者的邮件信箱无法接收此邮件</td>
    </tr>
    <tr>
        <td>收信者的信箱大小受到限制。</td>
        <td class="desc">1. 请缩小单笔邮件的大小，可将一封邮件切为多封邮件来传送 
    2.请收信端邮递员将收信上限提高 
    3. 若是还是无法寄送，可以考虑使用FTP的传输方式来传送</td>
    </tr>
    <tr>
        <td rowspan="2">530</td>
        <td>Authentication Is Required</td>
        <td class="desc">寄送之前，请做身份认证</td>
    </tr>
    <tr>
        <td>寄件端邮件服务器设定了一个寄信前必须做身份认证的机制。但是在邮件客户端程序比如Outlook里头您没有勾选输入认证数据的设定。</td>
        <td class="desc">1. 请在Outlook里的「我的服务器需要验证」打勾来启动SMTP AUTH的功能。</td>
    </tr>
    <tr>
        <td rowspan="2">530</td>
        <td>1. Your Server Has Been Blacklisted By the Recipient's Server 
    2. the Recipient's Mailbox Does Not Exist 
    3. the Message Cannot Be Delivered Due To a Configuration Error On the Server.  Please Contact Your Administrator</td>
        <td class="desc">1. 发件人的邮件服务器已经被置入收信者的黑名单之中 
    2. 收信者的信箱不存在 
    3. 由于邮件服务器上的设定错误造成您无法寄送信件，请联络您的网络管理员</td>
    </tr>
    <tr>
        <td>当出现这三种错误讯息时，寄件端邮件服务器已经被置入收信者的黑名单之中或是收信端信箱不存在。</td>
        <td class="desc">请联络收信者确认邮件地址或是请收信者联络邮递员将寄信者或是寄信端邮件服务器从黑名单中剔除。</td>
    </tr>
    <tr>
        <td rowspan="2">530 5.7.0</td>
        <td>Must Issue a Starttls Command First</td>
        <td class="desc">在开始寄信前，必须下一个STARTTLS的指令</td>
    </tr>
    <tr>
        <td>这错误讯息是您使用GMAIL时，若是没有输入身份验证的话，也有类似530 Authentication is required的错误讯息。</td>
        <td class="desc">请寄信者输入认证数据。</td>
    </tr>
    <tr>
        <td rowspan="2">535</td>
        <td>1. Error: Authentication Failed 
    2. Authentication Unsuccessful</td>
        <td class="desc">1. 错误讯息：验证失败 
    2. 验证不成功</td>
    </tr>
    <tr>
        <td>寄信端邮件服务器为了要防止垃圾信做出传递邮件的限制。</td>
        <td class="desc">可请邮递员设定SMTP AUTH的认证或是限定某个IP地址才可寄信的方式。</td>
    </tr>
    <tr>
        <td rowspan="2">541</td>
        <td>1. No Answer From Host
    2. Recipient Address Rejected - Access Denied (typically By the Recipient's Antispam Program / Appliance</td>
        <td class="desc">1. 收信者端没有回应
    2. 收信者端拒绝收信（通常是收信者端的反垃圾信程序造成的问题）</td>
    </tr>
    <tr>
        <td>1. 收件者主机无响应
    2. 收件者地址被拒</td>
        <td class="desc">请收信者通知网络管理者将寄信者加入白名单</td>
    </tr>
    <tr>
        <td rowspan="2">544</td>
        <td>Recipient Address Rejected: Relay Access Denied</td>
        <td class="desc">收信者邮件信箱被拒绝：传递邮件遭拒</td>
    </tr>
    <tr>
        <td>寄信端邮件服务器为了要防止垃圾信做出传递邮件的限制</td>
        <td class="desc">请在Outlook里的「我的 SMTP 服务器需要验证」打勾来启动 SMTP Auth 的功能
        设定 SMTP AUTH 的认证通过后再寄信，或是限定某个IP地址才可寄信的方式。</td>
    </tr>
    <tr>
        <td rowspan="2">550</td>
        <td>Unable To Relay For …</td>
        <td class="desc">此信件无法传递</td>
    </tr>
    <tr>
        <td>DNS指向设定错误造成无法解析收信端邮件服务器。</td>
        <td class="desc">请邮递员检测DNS是否正常。</td>
    </tr>
    <tr>
        <td rowspan="2">550</td>
        <td>Mailbox (xxx@xxx.xx) Not Found Or Inactivated</td>
        <td class="desc">信箱不存在或没被启用</td>
    </tr>
    <tr>
        <td>信箱不存在或没被启用。</td>
        <td class="desc">检查账号信箱是否已被删除或尚未启用</td>
    </tr>
    <tr>
        <td rowspan="2">550</td>
        <td>…relaying Denied</td>
        <td class="desc">电子邮件传递遭到拒绝</td>
    </tr>
    <tr>
        <td>寄信端邮件账号或是IP地址可能被收信端邮件服务器放入黑名单中。</td>
        <td class="desc">请与收信者通知邮递员将寄信者的IP地址或是寄信端邮件服务器IP地址从黑名单移除。</td>
    </tr>
    <tr>
        <td rowspan="2">550</td>
        <td>1. Requested Actions Not Taken As the Mailbox Is Unavailable 
    2. Not Our Customer 
    3. Invalid Recipient 
    4. No Such User Here 
    5.  Barack.obama@thiscompany.com, This Thiscompany.com Mailbox Does Not Exist – Giving Up 
    6. Account Not Available 
    7. Address Rejected 8. User Account Is Unavailable</td>
        <td class="desc">1. 所要求动作无法执行，信箱不存在 
    2. 不是我们的客户 
    3. 无效的收信者账号 
    4. 这里没有这个账号 
    5. THISCOMPANY.COM 这个账号不存在，放弃吧！
    6. 无此账号 
    7. 邮件地址被拒 
    8. 无此用户账号</td>
    </tr>
    <tr>
        <td>收件端邮件账号不存在、停用或被删除。</td>
        <td class="desc">发件人需向收信者确认正确的邮件地址</td>
    </tr>
    <tr>
        <td rowspan="2">550</td>
        <td>1. 550 Verification Failed For Xxx@xxx.xxx
    2. Previous (cached) Callout Verification Failure
    3. Sender Verify Failed</td>
        <td class="desc">1. 此账号 xxx@xxx.xxx 的身份核对失败 
    2. 前次存在快取里的身份核对失败
    3. 寄信者的身份核对失败</td>
    </tr>
    <tr>
        <td>通常意指寄信者已经被反垃圾信机制或是防火墙列入黑名单</td>
        <td class="desc">请收信者向邮递员反映，并把寄信者白名单化，并检查 spf 设定</td>
    </tr>
    <tr>
        <td rowspan="2">550</td>
        <td>Cyberoam Anti Spam Engine Has Identified This Email As a Spam. Refid:str=0001.0a0b0206.4ba7422c.01f5,ss=1,vtr=str,vl=0,pt =</td>
        <td class="desc">反垃圾信机制侦测并怀疑此信件为垃圾信</td>
    </tr>
    <tr>
        <td>通常发生在寄信端的防火墙或反垃圾信机制怀疑此封邮件可能是垃圾信因此阻挡下来。以防止垃圾信件流传到收件者端。</td>
        <td class="desc">请网络管理者对此信件放行。</td>
    </tr>
    <tr>
        <td rowspan="2">550</td>
        <td>Recipients' Mailbox Not Local And Mail Relay Is Not Enabled</td>
        <td class="desc">收信者的邮件信箱非本地信箱且无法做邮件转寄的动作</td>
    </tr>
    <tr>
        <td>寄信端邮件信箱和收信端邮件信箱不在同一网域内，无法寄信。</td>
        <td class="desc">寄信者请与网络管理员联系作适当的调整</td>
    </tr>
    <tr>
        <td rowspan="2">550</td>
        <td>The Sending Address Is Invalid</td>
        <td class="desc">寄信者的邮件地址无效</td>
    </tr>
    <tr>
        <td>寄信端邮件服务器的MX记录设定有误造成收件端的DNS系统无法解析寄件端的邮件地址，</td>
        <td class="desc">寄信者通知邮递员做检测并做修正。</td>
    </tr>
    <tr>
        <td rowspan="2">550</td>
        <td>Recipients Outside of Your Domain Where This Is Not Allowed</td>
        <td class="desc">寄信者邮件信箱和收信者邮件信箱不在同一网域内，无法寄信</td>
    </tr>
    <tr>
        <td>寄信者邮件信箱和收件者邮件信箱不在同一网域内，无法寄信。</td>
        <td class="desc">寄信者请与邮递员联系作适当的调整。</td>
    </tr>
    <tr>
        <td rowspan="2">550</td>
        <td>Smtp Authentication Required</td>
        <td class="desc">需要做SMTP身份认证来进行寄信的动作</td>
    </tr>
    <tr>
        <td>在Outlook或是Outlook Express里，SMTP AUTH若没有设定好，会出现此项错误讯息。</td>
        <td class="desc">在账号设定的「服务器」中点选「SMTP服务器需要认证」。</td>
    </tr>
    <tr>
        <td rowspan="2">550</td>
        <td>The Recipient's Server Is Down</td>
        <td class="desc">收信者的邮件服务器停机中</td>
    </tr>
    <tr>
        <td>收信端邮件服务器停机中。</td>
        <td class="desc">请收信者与网络管理员联络看看邮件服务器何时能够上线。</td>
    </tr>
    <tr>
        <td rowspan="2">550</td>
        <td>Change To Part of the Email Address To Achieve a Successful Delivery</td>
        <td class="desc">信件中的To必须改为正确的邮件账号</td>
    </tr>
    <tr>
        <td>有些公司已经改了自身的域名，因此要求发件人更正收信端邮件账号中的网域名部分。</td>
        <td class="desc">在邮件中更正邮件账号中的网域名之后重新寄送一次。</td>
    </tr>
    <tr>
        <td rowspan="2">550</td>
        <td>[suspend]mailbox Currently Suspended - Please Contact Correspondent Directly</td>
        <td class="desc">邮件信箱目前被停权，请自行与收信者用其他方式联络</td>
    </tr>
    <tr>
        <td>收信端邮件信箱目前被停权。</td>
        <td class="desc">请寄信者与收信者用其他方式取得联络</td>
    </tr>
    <tr>
        <td rowspan="2">550</td>
        <td>Incorrect From Address</td>
        <td class="desc">邮件中From的邮件地址不正确</td>
    </tr>
    <tr>
        <td>有些ISP禁止寄信者使用非自家维护的域名来寄信。</td>
        <td class="desc">请与ISP做沟通协调或是换一家ISP。</td>
    </tr>
    <tr>
        <td rowspan="2">550</td>
        <td>Mailbox Temporarily Disabled</td>
        <td class="desc">邮件信箱暂时被停用</td>
    </tr>
    <tr>
        <td>收信端邮件信箱可能已满尚未整理或是收信者尚未缴纳费用。</td>
        <td class="desc">请与收信者使用其他方式联系</td>
    </tr>
    <tr>
        <td rowspan="2">550</td>
        <td>1. Unrouteable Address</td>
        <td class="desc">1. 无效的邮件地址</td>
    </tr>
    <tr>
        <td>收信端的DNS服务器无法解析收信者网域</td>
        <td class="desc">检查收件者邮件地址是否正确</td>
    </tr>
    <tr>
        <td rowspan="2">550</td>
        <td>Mailbox Is Inactive</td>
        <td class="desc">邮件信箱尚未开通</td>
    </tr>
    <tr>
        <td>收信端邮件账号尚未开通。</td>
        <td class="desc">寄信者应通知收信者其邮件信箱尚未开通，并请ISP将信箱账号开通以供使用。</td>
    </tr>
    <tr>
        <td rowspan="2">550</td>
        <td>Relay Not Permitted</td>
        <td class="desc">禁止转寄</td>
    </tr>
    <tr>
        <td>收件方邮件服务器未正确设定管理之网域</td>
        <td class="desc">通知对方系统管理者</td>
    </tr>
    <tr>
        <td rowspan="2">550</td>
        <td>The Smtp Service To Send As Other Account Parties Is Not Valid For Your Account</td>
        <td class="desc">您的邮件账户设定不允许以他人名义发信</td>
    </tr>
    <tr>
        <td>发出信件的发件人账户与使用的 SMTP 账户不同</td>
        <td class="desc">请系统管理者更改此设定或发件人账户与SMTP账户以相同账户发信</td>
    </tr>
    <tr>
        <td rowspan="2">550 5.1.2</td>
        <td>Host Unknown – Host Cannot Be Found</td>
        <td class="desc">不明的主机 - 找不到收信者的邮件服务器主机</td>
    </tr>
    <tr>
        <td>DNS指向设定错误造成无法解析收信者端邮件服务器。</td>
        <td class="desc">请邮递员检测DNS是否正常。</td>
    </tr>
    <tr>
        <td rowspan="2">550 5.1.3</td>
        <td>Storedrv.submit; Invalid Recipient Address</td>
        <td class="desc">无效的收信者邮件地址</td>
    </tr>
    <tr>
        <td>此错误讯息为MS Exchange Server 2007特有。</td>
        <td class="desc">提醒使用者检查收信者的邮件地址是否符合语法规则</td>
    </tr>
    <tr>
        <td rowspan="2">550 5.4.1</td>
        <td>1. Recipient Address Rejected - Access Denied 
    2. Internet Security Systems' Proventia? Intrusion Prevention Appliance Blocked Forwarding of Message</td>
        <td class="desc">1. 收信者端拒绝收信 
    2. 因特网安全系统的入侵防止机制阻挡了邮件</td>
    </tr>
    <tr>
        <td>寄信端IP地址或是寄信端邮件服务器IP地址被列入黑名单中。</td>
        <td class="desc">请通知收信端邮件管理者将寄信端邮件账号加入白名单。</td>
    </tr>
    <tr>
        <td rowspan="2">550 5.7.1</td>
        <td>1. Unable To Relay For 
    2. Mail From Ip Address Refused By Blackhole Site Dialups.mail-abuse.org 
    3. Relaying Prohibited</td>
        <td class="desc">1. 寄信者的信件无法传递 
    2. 寄信者的IP地址已被锁定为黑名单 
    3. 禁止传送此信件</td>
    </tr>
    <tr>
        <td>当遇到这类讯息时，表示收信端邮件服务器将寄信端账号或是寄信端的网域名放入黑名单中。</td>
        <td class="desc">请与收信者端邮递员做沟通，加以漂白。</td>
    </tr>
    <tr>
        <td rowspan="2">550 5.7.1</td>
        <td>Our System Has Detected an Unusual Rate of Unsolicited Mail Originating From Your Ip Address. To Protect Our Users From Spam, Mail Sent From Your Ip Address Has Been Blocked. Please Visit Http://www.google.com/mail/help/bulk_mail.html To Review Our Bulk Email Senders Guidelines</td>
        <td class="desc">Google: 因发现不当的大量邮件来自你的 IP 地址，你的 IP 地址已被禁止寄入 GMAIL</td>
    </tr>
    <tr>
        <td>发送大量邮件至 Gmail</td>
        <td class="desc">依照大量邮件发送规范，重新检视你的电子邮件是否有不当之处．
    
   http://www.google.com/mail/help/bulk_mail.html</td>
    </tr>
    <tr>
        <td rowspan="2">551</td>
        <td>1. User Not Local Or Invalid Address –relay Denied 
    2. Delivery Not Allowed To Non-local Recipient</td>
        <td class="desc">1. 邮件服务器知道使用者不属于本地端拒绝做传递信的服务 
    2. 对于非本地的使用者不提供邮件传递的服务</td>
    </tr>
    <tr>
        <td>有些ISP为了要抵挡垃圾信乱飞的现象，他们索性对其他网域的使用者不提供传递信件的服务。</td>
        <td class="desc">1. 解决方式是打电话给这些ISP证明发件人非垃圾信制造者。
    2. 换一家ISP。</td>
    </tr>
    <tr>
        <td rowspan="2">552</td>
        <td>Requested Mail Action Aborted: Exceeded Storage Allocation</td>
        <td class="desc">所要求的动作中断：超出所分配的储存空间，邮件将退回给发件人</td>
    </tr>
    <tr>
        <td>收信端邮件信箱容量已达上限</td>
        <td class="desc">建议发件人通知收信者将信件清理一番</td>
    </tr>
    <tr>
        <td rowspan="2">552</td>
        <td>Size of the Incoming Message Exceeds the Incoming Size Limit</td>
        <td class="desc">新进信件的大小超过单笔新进信件的上限</td>
    </tr>
    <tr>
        <td>新进信件的大小超过单笔新进信件的上限。</td>
        <td class="desc">将欲寄信件分多笔寄出。2. 收信者与邮递员联络并将上限值做一个调整。</td>
    </tr>
    <tr>
        <td rowspan="2">552</td>
        <td>Too Many Recipients</td>
        <td class="desc">单封邮件中的收信者太多</td>
    </tr>
    <tr>
        <td>单封邮件中的收信者太多。</td>
        <td class="desc">建议分多笔邮件寄出。</td>
    </tr>
    <tr>
        <td rowspan="2">552</td>
        <td>Too Much Mail Data</td>
        <td class="desc">单封邮件中数据量过大</td>
    </tr>
    <tr>
        <td>单封邮件中数据量过大。</td>
        <td class="desc">建议将数据分散在多笔邮件中寄出。</td>
    </tr>
    <tr>
        <td rowspan="2">552</td>
        <td>Request Mail Action Aborted: Your are Not Allowed To Use Maillist Account</td>
        <td class="desc">所要求的邮件动作中断 - 不能用maillist的账号</td>
    </tr>
    <tr>
        <td>寄信者没有使用大量寄信功能的权限。</td>
        <td class="desc">请与邮递员确认权限。</td>
    </tr>
    <tr>
        <td rowspan="2">552</td>
        <td>Sorry, We Don't Allow Mail From Your Host</td>
        <td class="desc">寄信者所在主机不被允许寄信</td>
    </tr>
    <tr>
        <td>寄信者所在主机不被允许寄信。</td>
        <td class="desc">检查寄信端邮件账号是否被放进拒绝名单中。</td>
    </tr>
    <tr>
        <td rowspan="2">552</td>
        <td>Requested Mail Action Aborted:too Many Recipients, Limited Is 150</td>
        <td class="desc">收信者数量超过限制的150位</td>
    </tr>
    <tr>
        <td>单封邮件的收信者数量超过上限。</td>
        <td class="desc">1. 降低一次收信端邮件账号的数量。
    2. 分批寄信。</td>
    </tr>
    <tr>
        <td rowspan="2">552 5.1.1</td>
        <td>Sorry, Mailbox Alan@thiscompany.com Is Over Quota Temporarily</td>
        <td class="desc">很抱歉，Alan@ThisCompany.com这个信箱容量暂时超过上限</td>
    </tr>
    <tr>
        <td>收信端邮件账号信箱容量暂时超过上限。</td>
        <td class="desc">可通知收件者清理邮件信箱腾出空间来收信。</td>
    </tr>
    <tr>
        <td rowspan="2">552 5.2.3</td>
        <td>1. Data Size Exceeds Maximum Permitted 
    2. Message Exceeds Maximum Fixed Size</td>
        <td class="desc">1. 数据大小超出允许的最大值 
    2. 邮件超出预设的最大值</td>
    </tr>
    <tr>
        <td>单笔邮件数据大小还有信件大小超出允许的最大值。</td>
        <td class="desc">1.请缩小单笔邮件的大小，可将一封邮件切为多封邮件来传送 。
    2.请收信端通邮递员将收信上限提高。
    3. 若是还是无法寄送，可以考虑使用FTP的传输方式来传送</td>
    </tr>
    <tr>
        <td rowspan="2">552 5.3.4</td>
        <td>Error: Message File Too Big</td>
        <td class="desc">电子邮件讯息太大</td>
    </tr>
    <tr>
        <td>寄出的邮件可能包含过大的附件文件</td>
        <td class="desc">请缩小附件文件大小再试一次</td>
    </tr>
    <tr>
        <td rowspan="2">553</td>
        <td>1. Requested Action Not Taken: Mailbox Name Not Allowed [e.g. Mailbox Syntax Incorrect] 
    2. There Is an Invalid Email Address in the To, Cc Or Bcc Field of the Email Message 
    3. <email-address-you're-sending-to>. Addressee Unknown. Giving Up (553 5.3.0)</email-address-you're-sending-to></td>
        <td class="desc">1. 信件里的TO， CC， BCC有无效的收信者信箱地址 
    2. 不明的邮件地址，放弃传递</td>
    </tr>
    <tr>
        <td>因收信端邮件账号无效或错误出现此讯息</td>
        <td class="desc">请确认每一个收信端邮件账号都是有效的</td>
    </tr>
    <tr>
        <td rowspan="2">553</td>
        <td>Sorry, Relaying Denied From Your Location</td>
        <td class="desc">抱歉，无法从寄信者的所在地或是因特网联机发送信件</td>
    </tr>
    <tr>
        <td>有些ISP为了要抵挡垃圾信乱飞的现象，他们索性对其他网域的使用者不提供传递信件的服务。</td>
        <td class="desc">1. 解决方式是打电话给这些ISP证明发件人非垃圾信制造者。
    2. 换一家ISP。</td>
    </tr>
    <tr>
        <td rowspan="2">553</td>
        <td>1. Relay Restriction
    2. From &lt;&gt; Message Blocked
    3. Sorry, You are Not Allow To Use This Smtp To Relay Your Email
    4. Sorry, That Domain Isn't in My List of Allowed Rcpt Hosts</td>
        <td class="desc">1. 传送邮件是受到限制 
    2. 由发件人的身份寄信时遭到拒绝 
    3. 抱歉，发件人无法使用这个SMTP服务器来传递邮件 
    4. 抱歉，此网域不在SMTP服务器的允许寄送名单中</td>
    </tr>
    <tr>
        <td>在寄送信件之前必须先经过身份认证</td>
        <td class="desc">请在Outlook里的「我的 SMTP 服务器需要验证」打勾来启动 SMTP Auth 的功能</td>
    </tr>
    <tr>
        <td rowspan="2">553</td>
        <td>Authentication Is Required To Send Mail As</td>
        <td class="desc">在寄送信件之前必须先经过身份认证</td>
    </tr>
    <tr>
        <td>在Outlook或是Outlook Express里使用，若没有设定我的服务器需要验证，会出现此项错误讯息</td>
        <td class="desc">请在Outlook里的「我的 SMTP 服务器需要验证」打勾来启动 SMTP Auth 的功能</td>
    </tr>
    <tr>
        <td rowspan="2">553</td>
        <td>Mailbox Name Not Allowed</td>
        <td class="desc">收件人邮箱地址不合语法</td>
    </tr>
    <tr>
        <td>收信端邮件账号不合语法</td>
        <td class="desc">需检查收信端邮件账号是否正确</td>
    </tr>
    <tr>
        <td rowspan="2">553</td>
        <td>Sorry, Your Envelop Sender Is in My Bad Mail From List</td>
        <td class="desc">抱歉，寄信者电子邮件地址(邮件内)在黑名单中</td>
    </tr>
    <tr>
        <td>收信端邮件服务器限制了寄信端电子邮件地址</td>
        <td class="desc">1. 通知收信端邮递员将之放行
    2. 更改邮件的发件人电子邮件地址</td>
    </tr>
    <tr>
        <td rowspan="2">553</td>
        <td>Specified Domain Is Not Allowed</td>
        <td class="desc">收信端邮件服务器拒收来自特定网域的信件</td>
    </tr>
    <tr>
        <td>收信端邮件服务器拒收来自特定网域的信件</td>
        <td class="desc">请通知收信端邮递员将发件人所属网域名从黑名单中剔除</td>
    </tr>
    <tr>
        <td rowspan="2">553 5.1.3</td>
        <td>User Address Required!</td>
        <td class="desc">需要输入邮件账号</td>
    </tr>
    <tr>
        <td>信件中收信端邮件账号错误</td>
        <td class="desc">请确认收信端邮件账号输入无误</td>
    </tr>
    <tr>
        <td rowspan="2">553 5.1.3</td>
        <td>Invalid Local Part</td>
        <td class="desc">电子邮件收件者帐户部分错误</td>
    </tr>
    <tr>
        <td>可能使用了有 BUG 的邮件软件如 Outlook Express 导致寄出 <sp(空格)local_part@domain_part> 这样的邮件</sp(空格)local_part@domain_part></td>
        <td class="desc">重设通讯簿，尝试将问题信箱设定一个全名，或更换更好的邮件软件</td>
    </tr>
    <tr>
        <td rowspan="2">553 5.1.8</td>
        <td>Domain of Sender Address Does Not Exist</td>
        <td class="desc">发信者的网域不存在</td>
    </tr>
    <tr>
        <td>1. 寄信端的DNS服务器故障
    2. 收信端的DNS服务器故障
    3. 发件人信箱网域部分打错字</td>
        <td class="desc">检查邮件软件内设定的发件人电子邮件地址网域部分是否打错字</td>
    </tr>
    <tr>
        <td rowspan="2">554</td>
        <td>1. Transaction Failed
    2. Delivery Error: This User Doesn't Have a Yahoo.com Account
    3. Sorry Your Message To <email-address> Cannot Be Delivered. This Account Has Been Disabled Or Discontinued</email-address></td>
        <td class="desc">1. 传输失败 
    2. 收件者没有雅虎的邮件账号 
    3. 收件者的账号可能被停用或是收件者已经不在使用此邮件账号</td>
    </tr>
    <tr>
        <td>1. 收信端邮件账号错误</td>
        <td class="desc">1. 请检查收信端网域名
    2. 是否拼错字
    3. 请检查收信端邮件账号是否存在或是被停用</td>
    </tr>
    <tr>
        <td rowspan="2">554</td>
        <td>1. Smtp Relay Service Does Not Allow Your Ip Address To Relay Mail To Xxx@xxx.xxx
    2. Smtp Service Does Not Allow Your Ip Address
    3. Client Host Rejected: Access Denied</td>
        <td class="desc">1. SMTP寄信服务不允许寄信者的IP地址传递信件给 xxx@xxx.xxx
    2. SMTP寄信服务不允许寄信者的IP地址传递信件 
    3. 客户端被拒绝登入：存取拒绝</td>
    </tr>
    <tr>
        <td>寄信端邮件服务器为杜绝计算机病毒以及被当作垃圾信跳板，使用者必须经过 SMTP Auth 的身份认证才能寄信</td>
        <td class="desc">1. 请在Outlook里的「我的服务器需要验证」打勾来启动 SMTP Auth 的功能
    2. 强烈建议任何寄信者需经过 SMTP Auth 的身份认证，若需要 Open Relay 则需要手动加入寄信者的IP地址</td>
    </tr>
    <tr>
        <td rowspan="2">554</td>
        <td>1. (x.x.x.x) Was Found On One Or More Dnsbls, See Http://help.comcast.net/content/faq/bl000010
    2. Recipient Address Rejected
    3. Service Unavailable; Client Host (x.x.x.x) Blocked Using Barracuda Reputation; Http://recipientdomain.barracudacentral.com/q.cgi?ip= (554 5.7.1)
    4. Your Access To This Mail System Has Been Rejected Due To the Sending Mta's Poor Reputation. If You Believe That This Failure Is in Error, Please Contact the Intended Recipient Via Alternate Means</td>
        <td class="desc">1. 发件人的邮件服务器IP地址出现在DNSBLs中，详情请到下列网页察看： http://help.comcast.net/content/faq/BL000010 
    2. 拒绝收信者邮件地址 
    3. 寄信者的IP地址为反垃圾信机制所阻挡 
    4. 由于发件人的邮件服务器有发垃圾信的坏名誉纪录，收信者的邮件服务器拒收</td>
    </tr>
    <tr>
        <td>寄信端IP地址或邮件服务器的IP地址被放入黑名单</td>
        <td class="desc">1. 请与收信端邮件服务器管理员联系商讨是否可以将寄件端IP地址解除锁定
    2. 请寄信端邮递员或是所属ISP工作人员与RBL相关网站接洽讨论是否能从黑名单中除名</td>
    </tr>
    <tr>
        <td rowspan="2">554</td>
        <td>Your Ip (x.x.x.x) Is Dynamic Ip Address, Use Your Isp Smtp Server Instead</td>
        <td class="desc">您的IP地址视为动态IP地址，请使用您 ISP 的 SMTP 服务器</td>
    </tr>
    <tr>
        <td>收件端邮件服务器不接受动态IP地址上的邮件服务器</td>
        <td class="desc">请向您的ISP申请固定IP来架设邮件服务器</td>
    </tr>
    <tr>
        <td rowspan="2">554</td>
        <td>Your Ip (x.x.x.x) Was Listed in Dsbl - Please Visit Http://dsbl.org/listing?x.x.x.x For More Details</td>
        <td class="desc">寄信者的IP地址被收录在DSBL名单中，详情请看 http://dsbl.org/listing?x.x.x.x</td>
    </tr>
    <tr>
        <td>请不用担心这个黑名单，因为dsbl.org在2009年初已经下线。</td>
        <td class="desc">N/A</td>
    </tr>
    <tr>
        <td rowspan="2">554 5.3.0</td>
        <td>Mail Server Permanently Rejected Message</td>
        <td class="desc">邮件服务器永久地拒绝此邮件</td>
    </tr>
    <tr>
        <td>信件内容可能被对方过滤器阻挡</td>
        <td class="desc">请与收件端邮件管理者联系将发件人网域或IP地址加入白名单以跳过过滤机制</td>
    </tr>
    <tr>
        <td rowspan="2">554 5.7.1</td>
        <td>The File Xxx Has Been Blocked. File Quarantined As:b100493a.xxx</td>
        <td class="desc">档案XXX已被隔离放置于隔离区内。文件名为：b100493a.XXX。</td>
    </tr>
    <tr>
        <td>此档案极有可能含计算机病毒。</td>
        <td class="desc">请使用防病毒软件扫瞄处理。</td>
    </tr>
    <tr>
        <td rowspan="2">571</td>
        <td>1. Email Address We Do Not Relay
    2. the Following Addresses Had Permanent Delivery Errors: Xxx@xxx.xxx</td>
        <td class="desc">1. 我们无法为此收件者传递邮件(不提供转寄) 
    2. 此收信邮件账号有永久性收件上的问题：xxx@xxx.xxx</td>
    </tr>
    <tr>
        <td>原因一：收件者邮件服务器设定错误，误认自己不代管收件者网域
    原因二：寄信者没经过 SMTP Auth (我的外寄服务器(SMTP)需要认证) 的验证寄信模式 
    原因三：不被允许做寄信的动作
    原因四：寄信端邮件服务器在黑名单中</td>
        <td class="desc">原因一：收件者邮件服务器设定错误，误认自己不代管收件者网域
    原因二：寄信者没经过 SMTP Auth (我的外寄服务器(SMTP)需要认证) 的验证寄信模式 
    原因三：不被允许做寄信的动作
    原因四：寄信端邮件服务器在黑名单中</td>
    </tr>
</table>