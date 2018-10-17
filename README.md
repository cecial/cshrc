# cshrc
#cshrc setting

if ( $?prompt ) then 
    set prompt = "`hostname`: $cwd >"
endif

\# set execute search path 
setenv PATH "${PATH}:$HOME/script" 
\#set path = ($path \ 
\#             /$HOME/script 
\#              \) 

\# Highlight grep word
setenv GREP_OPTIONS --color=auto 

\# press tab to autofill file/dir, instead press Ctrl+D
set autolist 


alias cd 'cd \!*; set prompt = "`hostname`: $cwd >"'
