
cmake_minimum_required(VERSION 3.10)

project(exec09)

add_executable(exec09 6809.c command.c disk.c eon.c fileio.c imux.c ioexpand.c machine.c main.c miscsbc.c mmu.c monitor.c serial.c symtab.c timer.c wpc.c wpclib.c)
target_compile_definitions(exec09 PUBLIC HAVE_READLINE)
target_link_libraries(exec09 PUBLIC readline)

