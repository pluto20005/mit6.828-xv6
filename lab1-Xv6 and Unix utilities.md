# lab1:Xv6 and Unix utilities
## sleep
注意事项：
  
  1.在开始编码之前，请阅读 xv6 书籍的第 1 章。
  
  2.查看 user/ 目录下的其他程序（例如 user/echo.c、user/grep.c 和 user/rm.c），了解如何获取传递给程序的命令行参数。
  
  3.如果用户忘记传递参数，sleep 应该打印一条错误消息。
  
  4.命令行参数是以字符串形式传递的；您可以使用 atoi（参见 user/ulib.c）将其转换为整数。
  
  5.使用 sleep 系统调用。
  
  6.查看 kernel/sysproc.c 中实现 sleep 系统调用的 xv6 内核代码（查找 sys_sleep），查看 user/user.h 中用户程序可调用的 sleep 的 C 定义，以及查看 user/usys.S 中从用户代码跳转到内核执行 sleep 的汇编代码。
  
  7.确保 main 函数调用 exit() 以退出您的程序。
  
  8.将您的 sleep 程序添加到 Makefile 中的 UPROGS；完成此操作后，make qemu 将编译您的程序，并且您将能够从 xv6 shell 运行它。
