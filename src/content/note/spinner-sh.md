---
title: spinner.sh
description: spinner.sh 
publishDate: "2025-09-20T11:23:00Z"
---
```
printf "\e[?25l"
 spinner="◐◓◑◒"
 spin_i=0
 while true; do
   printf "\b%s" "${spinner:spin_i++%${#spinner}:1}"
   sleep 0.1
 done
```