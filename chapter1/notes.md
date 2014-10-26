c-h     ;; backspace
c-i     ;; tab
c-c     ;; break
c-u     ;; delete whole line
mail    ;; recv mails
mail Minami ;; mail to minami
who     ;; who's online
who am i ;; whoami
@       ;; cancel whole line
#       ;; backspace
stty -tabs ;; display tabs as space

c-s     ;; pause display to screen
c-q     ;; resume display to screen



execute sequential (readline -> shell -> command)

rm a.*
rm ch[1-57-9]*
sort <  filename  ;; read from file (< filename is interpreted by shell)


ls > ls.out ;; will cause ls.out in file ls.out (shell create and
interpret the file for ls first)

管道线上的程序实际上是同时运行的,而不是一个接一个的运行,这意味着管道线上的程序是
交互式的,内核对调度和同步做出处理,以便他们全部运行


ps -o pid,ppid,<fields> ;; the ppid of the command is always shell 

nohup command & ;; execute command even when the shell is exit




stty erase e kill k ;; delete and kill line (default is # and @)
stty erase '^h'
PS1="Dear?"
MAIL=/usr/mail/Minami ;; default dir for mail saving
PATH=$PATH:/new/dir   ;; add path
TERM=vim              ;; default editor type
d=/path/to/my/fav/dir ;; common used dir
cd $d                 ;; use downcase to determine your own variable 
export MAIL PATH TERM d ;; export to other application (except shell) to
read these variable








