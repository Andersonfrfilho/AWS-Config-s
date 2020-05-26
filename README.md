# AWS-Config-s

## Server for Aplication

## EC2 - Service Aws Eletronic computer two
### create VM
1. Open tab instances
   1. Launch instance
   2. Choice S.O
   3. Choice Hardware
   4. Choice details configurations
   5. Add storage
   6. Add Tags
   7. Configure Security group
   8. Review
   9. download key
### Access SSH 
2. Access Connect Linux with ssh (in tab instances choice VM select connect) use powershell in Windows.
   1. got to file where in file .pem
   2. propertys/securtity->advanced
     1. select users and remove, or Disable inhertance
     2. add ComputerName\\UserName
        * computarName show (myComputer->property)
        * UserName access c:\Users\nameUser
     3. select fullControl and ok
     4. click applied/ok
   3. ssh -i "ubuntuServer.pem" **ubuntu**@**ec2-100-26-174-190.compute-1.amazonaws.com**
### Access FTP   
3. ftp connect EC2 (Windows)
   1. use puttyGen
   2. click load select key_Of_AWS_EC2.pem
   3. save file.ppk
   4. open fileZilla/edit/config/SFTP
   5. Adicionar file key/addFile.key
   6. in input **Host** sftp://**ec2-100-26-174-190.compute-1.amazonaws.com**
   7. name user Nome de usuário: **ubuntu**
   8. connect.
  
  
  
  

