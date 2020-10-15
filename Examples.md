# Building and Running examples  

Instructions for Building the Example (assuming ACE, TAO, DDS, and MPC are installed and configured): 

Run Make Project Creator to generate build files: in vs developer command prompt

    cmd E:\opndds_\OpenDDS-master>setenv 

    cmd perl %ACE_ROOT%/bin/mwc.pl -type vc71 StockQuoter.mwc 

Configure –type vs2019 for visual studio 2019 

Open project using cmd 

    cmd devenv StockQuoter.sln 

Build the solution in vs - debug /win32 

## Server console 
    
    cmd E:\opndds_\OpenDDS-master\setenv 

    cmd E:\opndds_\OpenDDS-master\bin>.\DCPSInfoRepo -ORBEndpoint iiop://localhost:12345 -d domain_ids 

## Subscriber console  

    cmd E:\opndds_\OpenDDS-master\setenv 

    cmd E:\opndds_\OpenDDS-master\examples\DCPS\IntroductionToOpenDDS>subscriber -DCPSConfigFile dds_tcp_conf.ini 

## Publisher console 

    cmd E:\opndds_\OpenDDS-master\setenv 
    
    cmd E:\opndds_\OpenDDS-master\examples\DCPS\IntroductionToOpenDDS>publisher -DCPSConfigFile dds_tcp_conf.ini 
    
    
### extra 
https://github.com/wteamit/opendds-sample-01
