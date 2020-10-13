# OpenDDS
Quick start windows https://opendds.org/quickstart/GettingStartedWindows.html

## Installation Opendds 

Download repo 
https://github.com/objectcomputing/OpenDDS

Extract files 

Install strawberry perl 64 bit
http://strawberryperl.com/

open VS developer command prompt 

Navigate OpenDDS directory

    cmd configure // configure script will download ACE+TAO and configure it for your platform.

    cmd devenv DDS_TAOv2_all.sln // it must start the visual studio from this command prompt so it will inherit the correct environmental variables 

## Build  Opendds   

Build solution - Debug/ win32

## Run Opendds example    

VS developer comand promt

    Setenv // set the required environment variables before running Visual Studio
    Cd DevGuideExamples\DCPS\Messenger for C++ example
    Perl run_test.pl
    
Once new  developer command prompt window is opened use 

    cmd Setenv
