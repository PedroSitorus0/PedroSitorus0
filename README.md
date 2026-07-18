# Halo, Saya Pedro - Kernel Enthusiast

![Hikawa Hina](https://github.com/PedroSitorus0/PedroSitorus0/raw/main/hina-hikawa-cheers.gif)

## **Gak Tau Apa Ini Wok**

<details>
  <summary>Statistics</summary><br/>
  <p align="center">
    <a href="https://github.com/PedroSitorus0">
      <img width="60%" src="https://github-readme-stats-eight-theta.vercel.app/api?username=PedroSitorus0&show_icons=true&theme=dark&include_all_commits=true&count_private=true&icon_color=FFFFFF&bg_color=000000" />
      <img width="38%" src="https://github-readme-stats-eight-theta.vercel.app/api/top-langs/?username=PedroSitorus0&layout=compact&langs_count=10&theme=dark&bg_color=000000" />
      <img width="98.6%" src="https://github-readme-activity-graph.vercel.app/graph?username=PedroSitorus0&bg_color=000000&color=FFFFFF&point=FFFFFF&line=6CC644&area_color=6CC644&&area=true&radius=6&hide_title=true" />
    <a/>
  </p>
</details>

## **Tech Stack yang Bikin Meledak**

### **Low-Level Madness**
![Assembly](https://img.shields.io/badge/ASM-8B0000?style=for-the-badge&logo=assemblyscript&logoColor=white)
![C](https://img.shields.io/badge/C-000000?style=for-the-badge&logo=c&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?style=for-the-badge&logo=c%2B%2B&logoColor=white)

### **Web Development (Belum Punya Lambo)**
![PHP](https://img.shields.io/badge/PHP-777BB4?style=for-the-badge&logo=php&logoColor=white)


### **Scripting and Automation**
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Bash](https://img.shields.io/badge/Bash-4EAA25?style=for-the-badge&logo=gnu-bash&logoColor=white)


## **Thanks for stopping by**
![Hikawa Hina-2](https://github.com/PedroSitorus0/PedroSitorus0/raw/main/ruirins.gif)

## **Daily Reality**

```asm
section .data
    segfault_msg db "Segmentation fault (core dumped)", 0xA, 0
    true equ 1
    false equ 0

section .text
    global _start
    extern brain_is_functioning, code, drink_coffee, reboot_brain, printf

_start:

main_loop:
    call brain_is_functioning
    cmp eax, true
    je .call_code
    
    call drink_coffee
    jmp .end_if
    
.call_code:
    call code

.end_if:
    call check_exception
    cmp eax, true
    je .handle_exception
    
    jmp main_loop

.handle_exception:
    mov rdi, segfault_msg
    call printf
    
    ; Reboot brain
    call reboot_brain
    
    jmp main_loop

check_exception:
    mov eax, false
    ret

