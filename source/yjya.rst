第二章 应急预案
======================

2.1 ICCD配合主机实切步骤
--------------------------
主机升级停机，ICCD配合步骤::

  1、ICCD需要在主机下CP1C/CP1E （11.3.2.3/5）之前执行
  登录(生产IP为21.123.50.86）  
  第一步：以icpst01登陆(生产IP为21.123.50.86）服务器，执行admwin命令
  第二步：在出现的界面中输入柜员ID和密码。
  第三步：在出现的界面中选择“消息队列”
  第四步：在出现的界面中选择“禁止写消息队列”，弹出的界面中选择“PQM_ICHOST _1”。
  第五步：在弹出的界面中选择 禁止写(生产IP为21.123.50.90）服务器中中的带”EISS_L”和“EISS”的MQ
  第六步：此时将(生产IP为21.123.50.90）服务器中的MQ消息队列禁止写。
  查看队列状态为禁止写状态
  第一步：以icpst01登陆(生产IP为21.123.50.86）服务器，执行admwin命令
  第二步：在出现的界面中输入柜员ID和密码
  第三步：在出现的界面中选择“消息队列”
  第四步：在出现的界面中选择“应用队列信息”
  第五步：在出现的界面中找到(生产IP为21.123.50.90）中的带”EISS_L”和“EISS”的队列的MQ队列信息，状态为 INHIBITED

  登录(生产IP为21.123.50.88）  
  第一步：以icpst01登陆(生产IP为21.123.50.88）服务器，执行admwin命令
  第二步：在出现的界面中输入柜员ID和密码。
  第三步：在出现的界面中选择“消息队列”
  第四步：在出现的界面中选择“禁止写消息队列”，弹出的界面中选择“PQM_ICHOST _3”。
  第五步：在弹出的界面中选择 禁止写(生产IP为21.123.50.92）服务器中的带“EISS_L”和”EISS”的MQ
  第六步：此时将(生产IP为21.123.50.92）服务器中的MQ消息队列禁止写。
  查看队列状态为禁止写状态
  第一步：以icpst01登陆(生产IP为21.123.50.88）服务器，执行admwin命令
  第二步：在出现的界面中输入柜员ID和密码
  第三步：在出现的界面中选择“消息队列”
  第四步：在出现的界面中选择“应用队列信息”
  第五步：在出现的界面中找到(生产IP为21.123.50.92）中的带“EISS_L”和”EISS”的队列的MQ队列信息，状态为 INHIBITED  
  
  ACCS系统节点"CIP1AT11"之前执行
  登录（生产IP为21.123.50.86）
  第一步：以icpst01登录（生产IP为21.123.50.86）服务器，执行admwin命令
  第二步：在出现的界面中输入柜员ID和密码。
  第三步：再出现的界面中选择"消息队列"
  第四步：再出现的界面中选择"禁止写消息队列"，弹出的界面中依次选择"PQM_ICSWT_D_1和PQM_ICSWT_L_1".
  第五步：在弹出的界面中选择 禁止写（生产IP为21.123.50.86）服务器中带"ICPS.SWT*"的MQ
  第六步：此时将（生产IP为21.123.50.86）服务器中的MQ消息队列禁止写。
  查看队列状态为禁止写状态
  第一步：以icpst01登录（生产IP为21.123.50.86)服务器，执行admwin命令
  第二步：在出现的界面中输入柜员ID和密码。
  第三步：再出现的界面中选择"消息队列"
  第四步：在出现的界面中选择"应用队列信息"
  第五步：再出现的界面中找到（生产IP为21.123.50.86）中的带"ICPS.SWT*"的队列的MQ队列信息，状态为INHIBITED  
  
  ACCS系统节点"CIP1AT31" 之前执行
  登录（生产IP为21.123.50.88）
  第一步：以icpst01登录（生产IP为21.123.50.88）服务器，执行admwin命令
  第二步：在出现的界面中输入柜员ID和密码。
  第三步：再出现的界面中选择"消息队列"
  第四步：再出现的界面中选择"禁止写消息队列"，弹出的界面中依次选择"PQM_ICSWT_D_3和PQM_ICSWT_L_3".
  第五步：在弹出的界面中选择 禁止写（生产IP为21.123.50.88）服务器中带"ICPS.SWT*"的MQ
  第六步：此时将（生产IP为21.123.50.88）服务器中的MQ消息队列禁止写。
  查看队列状态为禁止写状态
  第一步：以icpst01登录（生产IP为21.123.50.88)服务器，执行admwin命令
  第二步：在出现的界面中输入柜员ID和密码。
  第三步：再出现的界面中选择"消息队列"
  第四步：在出现的界面中选择"应用队列信息"
  第五步：再出现的界面中找到（生产IP为21.123.50.88）中的带"ICPS.SWT*"的队列的MQ队列信息，状态为INHIBITED
  
  ICCD需要在主机启CP1C/CP1E （11.3.2.3/5）之后执行
  登录(生产IP为21.123.50.86）  
  第一步：以icpst01登陆(生产IP为21.123.50.86）服务器，执行admwin命令
  第二步：在出现的界面中输入柜员ID和密码。
  第三步：在出现的界面中选择“消息队列”
  第四步：在出现的界面中选择“允许写消息队列”，弹出的界面中选择“PQM_ICHOST _1”。
  第五步：在弹出的界面中选择 允许写(生产IP为21.123.50.90）服务器中中的带“EISS_L”和”EISS”的MQ
  第六步：此时将(生产IP为21.123.50.90）服务器中的MQ消息队列允许写。
  查看队列状态为允许写状态
  第一步：以icpst01登陆(生产IP为21.123.50.86）服务器，执行admwin命令
  第二步：在出现的界面中输入柜员ID和密码
  第三步：在出现的界面中选择“消息队列”
  第四步：在出现的界面中选择“应用队列信息”
  第五步：在出现的界面中找到(生产IP为21.123.50.90）中的带“EISS_L”和”EISS”的队列的MQ队列信息，状态为 ALLOWED
  
  登录(生产IP为21.123.50.88）  
  第一步：以icpst01登陆(生产IP为21.123.50.88）服务器，执行admwin命令
  第二步：在出现的界面中输入柜员ID和密码。
  第三步：在出现的界面中选择“消息队列”
  第四步：在出现的界面中选择“允许写消息队列”，弹出的界面中选择“PQM_ICHOST _3”。
  第五步：在弹出的界面中选择 允许写(生产IP为21.123.50.92）服务器中中的带“EISS_L”和”EISS”的MQ
  第六步：此时将(生产IP为21.123.50.92）服务器中的MQ消息队列允许写。
  查看队列状态为允许写状态
  第一步：以icpst01登陆(生产IP为21.123.50.88）服务器，执行admwin命令
  第二步：在出现的界面中输入柜员ID和密码
  第三步：在出现的界面中选择“消息队列”
  第四步：在出现的界面中选择“应用队列信息”
  第五步：在出现的界面中找到(生产IP为21.123.50.92）中的带“EISS_L”和”EISS”的队列的MQ队列信息，状态为 ALLOWED"  
  
  ACCS系统升级的节点"CIP1AT11" 漂移到其他节点之后，ICCD恢复与此节点的交易传输
  登录（生产IP为21.123.50.86）
  第一步：以icpst01登录（生产IP为21.123.50.86）服务器，执行admwin命令
  第二步：在出现的界面中输入柜员ID和密码。
  第三步：再出现的界面中选择"消息队列"
  第四步：再出现的界面中选择"允许写消息队列"，弹出的界面中依次选择"PQM_ICSWT_D_1和PQM_ICSWT_L_1".
  第五步：在弹出的界面中选择 允许写（生产IP为21.123.50.86）服务器中带"ICPS.SWT*"的MQ
  第六步：此时将（生产IP为21.123.50.86）服务器中的MQ消息队列禁止写。
  查看队列状态为禁止写状态
  第一步：以icpst01登录（生产IP为21.123.50.86)服务器，执行admwin命令
  第二步：在出现的界面中输入柜员ID和密码。
  第三步：再出现的界面中选择"消息队列"
  第四步：在出现的界面中选择"应用队列信息"
  第五步：再出现的界面中找到（生产IP为21.123.50.86）中的带"ICPS.SWT*"的队列的MQ队列信息，状态为ALLOWED  
  
  ACCS系统升级的节点"CIP1AT31" 漂移到其他节点之后，ICCD恢复与此节点的交易传输
  登录（生产IP为21.123.50.88）
  第一步：以icpst01登录（生产IP为21.123.50.88）服务器，执行admwin命令
  第二步：在出现的界面中输入柜员ID和密码。
  第三步：再出现的界面中选择"消息队列"
  第四步：再出现的界面中选择"允许写消息队列"，弹出的界面中依次选择"PQM_ICSWT_D_3和PQM_ICSWT_L_3".
  第五步：在弹出的界面中选择 允许写（生产IP为21.123.50.88）服务器中带"ICPS.SWT*"的MQ
  第六步：此时将（生产IP为21.123.50.88）服务器中的MQ消息队列禁止写。
  查看队列状态为禁止写状态
  第一步：以icpst01登录（生产IP为21.123.50.88)服务器，执行admwin命令
  第二步：在出现的界面中输入柜员ID和密码。
  第三步：再出现的界面中选择"消息队列"
  第四步：在出现的界面中选择"应用队列信息"
  第五步：再出现的界面中找到（生产IP为21.123.50.88）中的带"ICPS.SWT*"的队列的MQ队列信息，状态为ALLOWED
  
  
  -------------------------------------------------------------------------------------------------------------------------
  
  2、ICCD需要在主机下CP1D/CP1F （11.3.2.4/6）之前执行
  登录(生产IP为21.123.50.86）  
  第一步：以icpst01登陆(生产IP为21.123.50.86）服务器，执行admwin命令
  第二步：在出现的界面中输入柜员ID和密码。
  第三步：在出现的界面中选择“消息队列”
  第四步：在出现的界面中选择“禁止写消息队列”，弹出的界面中选择“PQM_ICHOST _2”。
  第五步：在弹出的界面中选择 禁止写(生产IP为21.123.50.91）服务器中中的带“EISS_L”和”EISS”的MQ
  第六步：此时将(生产IP为21.123.50.91）服务器中的MQ消息队列禁止写。
  查看队列状态为禁止写状态
  第一步：以icpst01登陆(生产IP为21.123.50.86）服务器，执行admwin命令
  第二步：在出现的界面中输入柜员ID和密码
  第三步：在出现的界面中选择“消息队列”
  第四步：在出现的界面中选择“应用队列信息”
  第五步：在出现的界面中找到(生产IP为21.123.50.91）中的带“EISS_L”和”EISS”的队列的MQ队列信息，状态为 INHIBITED  
  
  登录(生产IP为21.123.50.88）  
  第一步：以icpst01登陆(生产IP为21.123.50.88）服务器，执行admwin命令
  第二步：在出现的界面中输入柜员ID和密码。
  第三步：在出现的界面中选择“消息队列”
  第四步：在出现的界面中选择“禁止写消息队列”，弹出的界面中选择“PQM_ICHOST _4”。
  第五步：在弹出的界面中选择 禁止写(生产IP为21.123.50.93）服务器中的带“EISS_L”和”EISS”的MQ
  第六步：此时将(生产IP为21.123.50.93）服务器中的MQ消息队列禁止写。
  查看队列状态为禁止写状态
  第一步：以icpst01登陆(生产IP为21.123.50.88）服务器，执行admwin命令
  第二步：在出现的界面中输入柜员ID和密码
  第三步：在出现的界面中选择“消息队列”
  第四步：在出现的界面中选择“应用队列信息”
  第五步：在出现的界面中找到(生产IP为21.123.50.93）中的带“EISS_L”和”EISS”的队列的MQ队列信息，状态为 INHIBITED
  
  ACCS系统节点"CIP1AT21" (第一次隔离下机）之前执行
  登录（生产IP为21.123.50.87）
  第一步：以icpst01登录（生产IP为21.123.50.87）服务器，执行admwin命令
  第二步：在出现的界面中输入柜员ID和密码。
  第三步：再出现的界面中选择"消息队列"
  第四步：再出现的界面中选择"禁止写消息队列"，弹出的界面中依次选择"PQM_ICSWT_D_2和PQM_ICSWT_L_2".
  第五步：在弹出的界面中选择 禁止写（生产IP为21.123.50.87）服务器中带"ICPS.SWT*"的MQ
  第六步：此时将（生产IP为21.123.50.87）服务器中的MQ消息队列禁止写。
  查看队列状态为禁止写状态
  第一步：以icpst01登录（生产IP为21.123.50.87)服务器，执行admwin命令
  第二步：在出现的界面中输入柜员ID和密码。
  第三步：再出现的界面中选择"消息队列"
  第四步：在出现的界面中选择"应用队列信息"
  第五步：再出现的界面中找到（生产IP为21.123.50.87）中的带"ICPS.SWT*"的队列的MQ队列信息，状态为INHIBITED
  
  ACCS系统节点"CIP1AT41" (第一次隔离下机）之前执行
  登录（生产IP为21.123.50.89）
  第一步：以icpst01登录（生产IP为21.123.50.89）服务器，执行admwin命令
  第二步：在出现的界面中输入柜员ID和密码。
  第三步：再出现的界面中选择"消息队列"
  第四步：再出现的界面中选择"禁止写消息队列"，弹出的界面中依次选择"PQM_ICSWT_D_4和PQM_ICSWT_L_4".
  第五步：在弹出的界面中选择 禁止写（生产IP为21.123.50.89）服务器中带"ICPS.SWT*"的MQ
  第六步：此时将（生产IP为21.123.50.89）服务器中的MQ消息队列禁止写。
  查看队列状态为禁止写状态
  第一步：以icpst01登录（生产IP为21.123.50.89)服务器，执行admwin命令
  第二步：在出现的界面中输入柜员ID和密码。
  第三步：再出现的界面中选择"消息队列"
  第四步：在出现的界面中选择"应用队列信息"
  第五步：再出现的界面中找到（生产IP为21.123.50.89）中的带"ICPS.SWT*"的队列的MQ队列信息，状态为INHIBITED  
  
  ICCD需要在主机启CP1D/CP1F （11.3.2.4/6）之后执行
  登录(生产IP为21.123.50.86）  
  第一步：以icpst01登陆(生产IP为21.123.50.86）服务器，执行admwin命令
  第二步：在出现的界面中输入柜员ID和密码。
  第三步：在出现的界面中选择“消息队列”
  第四步：在出现的界面中选择“允许写消息队列”，弹出的界面中选择“PQM_ICHOST _2”。
  第五步：在弹出的界面中选择 允许写(生产IP为21.123.50.91）服务器中中的带“EISS_L”和”EISS”的MQ
  第六步：此时将(生产IP为21.123.50.91）服务器中的MQ消息队列允许写。
  查看队列状态为允许写状态
  第一步：以icpst01登陆(生产IP为21.123.50.86）服务器，执行admwin命令
  第二步：在出现的界面中输入柜员ID和密码
  第三步：在出现的界面中选择“消息队列”
  第四步：在出现的界面中选择“应用队列信息”
  第五步：在出现的界面中找到(生产IP为21.123.50.91）中的带“EISS_L”和”EISS”的队列的MQ队列信息，状态为 ALLOWED  
  
  登录(生产IP为21.123.50.88）  
  第一步：以icpst01登陆(生产IP为21.123.50.88）服务器，执行admwin命令
  第二步：在出现的界面中输入柜员ID和密码。
  第三步：在出现的界面中选择“消息队列”
  第四步：在出现的界面中选择“允许写消息队列”，弹出的界面中选择“PQM_ICHOST _4”。
  第五步：在弹出的界面中选择 允许写(生产IP为21.123.50.93）服务器中中的带“EISS_L”和”EISS”的MQ
  第六步：此时将(生产IP为21.123.50.93）服务器中的MQ消息队列允许写。
  查看队列状态为允许写状态
  第一步：以icpst01登陆(生产IP为21.123.50.88）服务器，执行admwin命令
  第二步：在出现的界面中输入柜员ID和密码
  第三步：在出现的界面中选择“消息队列”
  第四步：在出现的界面中选择“应用队列信息”
  第五步：在出现的界面中找到(生产IP为21.123.50.93）中的带“EISS_L”和”EISS”的队列的MQ队列信息，状态为 ALLOWED"  
  
  ACCS系统升级的节点"CIP1AT21" 漂移到其他节点之后，ICCD恢复与此节点的交易传输
  登录（生产IP为21.123.50.87）
  第一步：以icpst01登录（生产IP为21.123.50.87）服务器，执行admwin命令
  第二步：在出现的界面中输入柜员ID和密码。
  第三步：再出现的界面中选择"消息队列"
  第四步：再出现的界面中选择"允许写消息队列"，弹出的界面中依次选择"PQM_ICSWT_D_2和PQM_ICSWT_L_2".
  第五步：在弹出的界面中选择 允许写（生产IP为21.123.50.87）服务器中带"ICPS.SWT*"的MQ
  第六步：此时将（生产IP为21.123.50.87）服务器中的MQ消息队列禁止写。
  查看队列状态为禁止写状态
  第一步：以icpst01登录（生产IP为21.123.50.87)服务器，执行admwin命令
  第二步：在出现的界面中输入柜员ID和密码。
  第三步：再出现的界面中选择"消息队列"
  第四步：在出现的界面中选择"应用队列信息"
  第五步：再出现的界面中找到（生产IP为21.123.50.87）中的带"ICPS.SWT*"的队列的MQ队列信息，状态为ALLOWED  
  
  ACCS系统升级的节点"CIP1AT41" 漂移到其他节点之后，ICCD恢复与此节点的交易传输
  登录（生产IP为21.123.50.89）
  第一步：以icpst01登录（生产IP为21.123.50.89）服务器，执行admwin命令
  第二步：在出现的界面中输入柜员ID和密码。
  第三步：再出现的界面中选择"消息队列"
  第四步：再出现的界面中选择"允许写消息队列"，弹出的界面中依次选择"PQM_ICSWT_D_4和PQM_ICSWT_L_4".
  第五步：在弹出的界面中选择 允许写（生产IP为21.123.50.89）服务器中带"ICPS.SWT*"的MQ
  第六步：此时将（生产IP为21.123.50.89）服务器中的MQ消息队列禁止写。
  查看队列状态为禁止写状态
  第一步：以icpst01登录（生产IP为21.123.50.89)服务器，执行admwin命令
  第二步：在出现的界面中输入柜员ID和密码。
  第三步：再出现的界面中选择"消息队列"
  第四步：在出现的界面中选择"应用队列信息"
  第五步：再出现的界面中找到（生产IP为21.123.50.89）中的带"ICPS.SWT*"的队列的MQ队列信息，状态为ALLOWED
  


2.2 ICCD与EISS之间MQ异常应急方案
------------------------------------

  ICCD与EISS之间MQ异常应急方案:                             
                                    
  .. image:: ./images/eiss_mq.PNG      
  ..                                
   :width: 200px
 
                

