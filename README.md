# AWS-Config-s

## Server for Aplication

## EC2 - Service Aws Eletronic computer two
### create VM
1. Open tab instances
   * Launch instance
   * Choice S.O
   * Choice Hardware
   * Choice details configurations
   * Add storage
   * Add Tags
   * Configure Security group
   * Review
   * download key
### Access SSH (<https://www.youtube.com/watch?v=N9t2RzmHta8>)
2. Access Connect Linux with ssh (in tab instances choice VM select connect) use powershell in Windows.
   * got to file where in file .pem
   * propertys/securtity->advanced
     * select users and remove, or Disable inhertance
     * add ComputerName\\UserName
        * computarName show (myComputer->property)
        * UserName access c:\Users\nameUser
     * select fullControl and ok
     * click applied/ok
   * ssh -i "ubuntuServer.pem" **ubuntu**@**ec2-100-26-174-190.compute-1.amazonaws.com**
   * **install nvm**
   2.1. install nvm 
         * use command in terminal 
           ```curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.35.3/install.sh | bash```
         * definindo environment variable linux
           ```export NVM_DIR="$([ -z "${XDG_CONFIG_HOME-}" ] && printf %s "${HOME}/.nvm" || printf %s "${XDG_CONFIG_HOME}/nvm")" [ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh" # This loads nvm```
         * install version node in nvm, case using specific version change lts for number version
           ```nvm install --lts```
         * use version instaled
           ```nvm use --lts```
           * show versions
             ```nvm list```

### Access FTP   (<https://youtu.be/W6BBrz3jKw8>)
3. ftp connect EC2 (Windows)
   
   * use puttyGen
   * click load select key_Of_AWS_EC2.pem
   * save **private key** file.ppk
   * download **fileZilla**
   * open fileZilla/edit/config/SFTP
   * Adicionar file key/addFile.key
   * in input **Host** sftp://**ec2-100-26-174-190.compute-1.amazonaws.com**
   * name user Nome de usuário: **ubuntu**
   * connect.
     * case problem's with permission denied <https://stackoverflow.com/questions/19648712/amazon-aws-filezilla-transfer-permission-denied>
     * use comand in terminal machine ec2. 
       * case not work using ```sudo su``` and back the comands.
       - ```chown -R ec2-user /var/www/html```
       - ```chmod -R 755 /var/www/html```
  
  
  
  

