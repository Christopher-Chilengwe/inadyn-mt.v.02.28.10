When inadyn-mt is installed as a service, its registry parameters are 
set so as to look for inadyn-mt.conf in the "module" directory (the 
directory from which inadyn-mt was run to install it as a service), i.e.,
.\inadyn-mt.conf.

To install as a service, you can run install_inadyn-mt_service.bat from
the present directory, or you can install from the present directory at
a DOS prompt with:

inadyn-mt -i

Start from the Windows service command manager, or from command prompt with:

inadyn-mt -s

Stop from the Windows service command manager, or from command prompt with:

inadyn-mt -e

Uninstall by running remove_inadyn-mt_service.bat, or from the command prompt
with:

inadyn-mt -x

Generally you don't need to bother with .reg files here, but if you want
to change registry parameters, for instance to set as in command line fashion
with or without an input file, take a look at them (right click, and edit, or
'open with') - at the very least, they'll show you where to find inadyn-mt in 
the registry.

You can run inadyn-mt as a "console" application from the command line with:

inadyn-mt --input_file .\inadyn-mt.conf
