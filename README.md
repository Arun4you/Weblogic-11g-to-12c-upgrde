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
