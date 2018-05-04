pypi
=================

https://pypi.org/project/multiJump/

wiki
=================

https://github.com/seqyuan/multiJump/wiki

Install multiJump
=================
安装示例
::

    pip3 install multiJump

class
=================

::

    calss jump_exe_cmd(mid_host_ip = None, mid_port=22, mid_username=None, mid_password=None,,mid_connect_timeout=60,cmd_mid = None, end_host_ip = None, end_port = None, cmd_end_to_exe = None, end_host_user = None)

The jump_exe_cmd object provides a methods intended for jump to mid IP rum cmd, and then jump to the end IP from mid IP rum cmd.

::

    __init__(mid_host_ip = None, mid_port=22, mid_username=None, mid_password=None, mid_connect_timeout=60 , cmd_mid = None, end_host_ip = None, end_port = None, cmd_end_to_exe = None, end_host_user = None)

Create an object.

**Parameters:** 

| **mid_host_ip** – mid_host_ip
| **mid_port** – mid_port
| **mid_username** – mid_username
| **mid_password** – mid_password
| **mid_connect_timeout** – mid_connect_timeout
| **cmd_mid** – cmd_mid
| **end_host_ip** – end_host_ip
| **end_port** – end_port
| **cmd_end_to_exe** – cmd_end_to_exe
| **end_host_user** – end_host_user
                
::

    exe_cmd()

Connect the multiple IP then run mid and end command.