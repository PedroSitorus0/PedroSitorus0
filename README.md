# Halo, Saya Pedro - The Stressed Coder - Saya butuh tidur

![Header](https://capsule-render.vercel.app/api?type=waving&color=gradient&height=200&section=header&text=My%20Brain%20is%20Compiling...&fontSize=30&fontColor=000000)

## **Tech Stack yang Bikin Pusing**

### **Low-Level Madness**
![Assembly](https://img.shields.io/badge/ASM-8B0000?style=for-the-badge&logo=assemblyscript&logoColor=white)
![C](https://img.shields.io/badge/C-000000?style=for-the-badge&logo=c&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?style=for-the-badge&logo=c%2B%2B&logoColor=white)

### **Web Development (Belum Punya Lambo)**
![PHP](https://img.shields.io/badge/PHP-777BB4?style=for-the-badge&logo=php&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)

### **Scripting & Automation**
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Bash](https://img.shields.io/badge/Bash-4EAA25?style=for-the-badge&logo=gnu-bash&logoColor=white)

## GitHub Stats yang Mencerminkan Stress Level

[](https://github-readme-stats.vercel.app/api?username=PedroSitorus0&show_icons=true&theme=dark&bg_color=0d1117&hide_border=true&include_all_commits=true)

![](https://github-readme-stats.vercel.app/api/top-langs/?username=PedroSitorus0&layout=compact&theme=dark&bg_color=0d1117&hide_border=true&langs_count=6)

![GitHub Streak](https://streak-stats.demolab.com?user=PedroSitorus0&theme=dark&background=0d1117&hide_border=true)

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
