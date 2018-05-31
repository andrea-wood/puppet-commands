# puppet-commands

# Create user with password
openssl passwd -1  
# Enter your password here 
Password: 
Verifying - Password: 
$1$HTumvYUGYUGwsxQxCp3F/nGc4DCYM
 
 # Inser the password into resource:
 user { 'TestUser': 
  ensure   => present,
  password => '$1$HTumvYUGYUGwsxQxCp3F/nGc4DCYM',
}
