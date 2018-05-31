# puppet-commands

# Create user with password
openssl passwd -1  
# Enter your password here 
Password: <br />
Verifying - Password: <br />
$1$HTumvYUGYUGwsxQxCp3F/nGc4DCYM<br />
 
 # Inser the password into resource:
 user { 'TestUser': <br />
  ensure   => present,<br />
  password => '$1$HTumvYUGYUGwsxQxCp3F/nGc4DCYM',<br />
}
