# lpac, The GNU/Linux Package Manager

lpac (**l**inux **pac**kager), is a modern and lightweight package manager, written in Go, focused on keeping a clean GNU/Linux system.

## Why?

> In my eyes, for the next big (and not-so-big) reasons:

### A cleaner system

Most UN\*X package managers, put all the installed packages and their dependencies inside /usr/bin, /usr/lib or /usr/include without distinguishing any file from the system files, making these directories: "dirty directories". Finishing with a system filled with dependencies that you don't known why them are there.

When you want to uninstall a package, some packages and their dependencies aren't removed nor the configuration files, unless you instruct your package manager to behave as such. lpac reverses this behavior and behaves like that by default.

lpac, forces you to keep a structure and a traking of installed packages and its dependencies, [isolating its dependencies](#) if just one package depends on them.

### An experiment

As unique developer of this software at this moment, I want to know how a package manager works, so the best way is implementing one from scratch.

### Practise my Go abilities

I'm relatively new to the Go language, as I think it produces powerful and clean software, is a good idea to practice it.