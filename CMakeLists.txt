
cmake_minimum_required(VERSION 3.10)

project(exec09)

add_executable(m6809-run 6809.c command.c disk.c eon.c fileio.c imux.c ioexpand.c machine.c main.c miscsbc.c mmu.c monitor.c serial.c symtab.c timer.c wpc.c wpclib.c)
target_compile_definitions(m6809-run PUBLIC HAVE_READLINE)
target_link_libraries(m6809-run PUBLIC readline)

