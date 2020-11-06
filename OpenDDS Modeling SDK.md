A guide to use modelung sdk and create application code and run with perl script

## Intro

https://opendds.org/about/modeling/

https://opendds.org/about/modeling/modeling_capture.html

https://opendds.org/about/modeling/modeling_program.html

## to start with application code examples 

https://github.com/objectcomputing/OpenDDS/tree/master/tools/modeling/tests/Messenger

## steps

modeling sdk builds suppoers eclipse 3.x and 4.4 only 

setup modeling sdk to eclipse 4.4 

devguide chapter-11 explains installation 

after installation creaste new model project 

then refer help in eclipse - detialed desciption on model creastion / validation and code generation 

codegen transport -> add tcp child

codegen output files

<model>_t.h and .cpp
<model>_traits.h and .cpp
<model>.idl
<model>.mpc
<model>.mpb
<model>_paths.mpb

.MWC should created manualy
get acopy of  run_test.pl from above file 

locate created model files in dds repo

    dev cmd promt -> setenv
    dev cmd promt -> perl %ACE_ROOT%\bin\mwc.pl -type vs2019 SafGenInt.mwc 
    build with vs 

this will create reuiqred typeSupport , export header and other files 

to create application code and application .MPC refer  link https://github.com/objectcomputing/OpenDDS/tree/master/tools/modeling/tests/Messenger
copy pub.cpp and sub.cpp edit accordingly (namespaces according to model etc...)

    dev cmd promt -> setenv
    dev cmd promt -> perl %ACE_ROOT%\bin\mwc.pl -type vs2019 SafGenInt.mwc 
    dev cmd promt -> devenv <model>.sln 
    dev cmd promt -> run_test.pl



