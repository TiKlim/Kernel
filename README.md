# Kernel
## О проекте
"Написать ядро с поддержкой клавиатуры и экрана"
![изображение](https://github.com/TiKlim/Kernel/assets/114877716/a4e6a504-4c82-4bd4-83be-5ac226ac2bde

## Запуск:
1. Скачайте файлы из репозитория;

2. Загрузить утилиты gcc, nasm, qemu ;

3. Собрать проект:

   a. Выполнить команду: nasm -f elf32 kernel.asm -o kasm.o ;

   b. Выполнить команду: gcc -m32 -c kernel.c -o kc.o ;

   c. Выполнить команду: gcc -fno-stack-protector -m32 -c kernel.c -o kc.o ;

   d. Выполнить команду: ld -m elf_i386 -T link.ld -o kernel kasm.o kc.o .

5. Запустить на эмуляторе: qemu-system-i386 -kernel kernel .

## Контакты
klim.timofeev.04@mail.ru

Тимофеев Клим, 2024.
