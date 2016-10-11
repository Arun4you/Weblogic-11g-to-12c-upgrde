# Weblogic-11g-to-12c-upgrde

tar -cf output.tar Domain-name
 
tar -xf pnbr3dev.tar
 
copy the same java directory
 
edit config.xml both port/hostname
 
-Dweblogic.configuration.schemaValidationEnabled=false
 
copy /opt/grd/MercuryDiagnostics/
 
setDomainEnv.sh
 
./startAdminServer.sh
 
./startManagedWebLogic.sh
 
/opt/grd/Oracle/Middleware/jdk1.6.0_85/jre/lib/management - all files

#PACK and UNPACK command

./pack.sh -domain=/opt/grd/Oracle12.1.3/user_projects/domains/WL12cTesting -template=WL12cTesting.jar -template_name="WL_pack"

[grd@dayrhegrdd008 bin]$./unpack.sh -template=WL12cTesting.jar -domain=/opt/grd/Oracle12.1.3/user_projects/domains/WL12cTesting

Include manages servers
 
./pack.sh -managed=true -domain=/opt/grd/Oracle/Middleware-INT/user_projects/domains/ogrdsdevr2_pb -template=CodingINT.jar -template_name="INT_pack"

