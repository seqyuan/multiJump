## Example
```
import sys
import getpass
sys.path.append('/home/yuanzan/test/multiJump_test/lib/python3.3/site-packages/multiJump')
import multiJump as mJ

mid_cli_usr = getpass.getuser()
mid_cmd = 'scp -r -P 50732 /home/yuanzan/test/multiJump_test/KJ-DB-PM-GD160041-01-t-2018-P10673.tar.gz /home/yuanzan/test/multiJump_test/email_content.html {}@192.168.60.188:/home/yuanzan/12489/'.format(mid_cli_usr)
end_cmd = '/home/yuanzan/sendmail/sendEmail zanyuan@genome.cn zanyuan@genome.cn 【反馈邮件】NCC-1701U.S.S.EnterpriseHi-C文库建库测序分析任务单 ~/12489/email_content.html ~/12489/KJ-DB-PM-GD160041-01-t-2018-P10673.tar.gz && rm -rf ~/12489/'

jump_obj = mJ.jump_exe_cmd(mid_host_ip='c0008', end_host_ip='192.168.60.188', end_port=50732, cmd_mid=None , cmd_end_to_exe='mkdir ~/12489', mid_username=mid_cli_usr, end_host_user=mid_cli_usr)
jump_obj.exe_cmd()

jump_obj2 = mJ.jump_exe_cmd(mid_host_ip='c0008', end_host_ip='192.168.60.188', end_port=50732, cmd_mid=mid_cmd , cmd_end_to_exe=end_cmd, mid_username=mid_cli_usr, end_host_user=mid_cli_usr)
jump_obj2.exe_cmd()

```