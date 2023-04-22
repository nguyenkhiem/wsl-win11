# wsl-win11

# install wsl

App -> Optional features -> More Windows features -> checked box "Windows Subsystem for Linux" 

# change drive
```console
PS C:\Users\khiem> wsl --list -v
  NAME      STATE           VERSION
* Ubuntu    Stopped         2
PS C:\Users\khiem> wsl --export Ubuntu "E:\wsl\ubuntu-ex.tar"
Export in progress, this may take a few minutes.
The operation completed successfully.
PS C:\Users\khiem> wsl --unregister Ubuntu
Unregistering.
The operation completed successfully.
PS C:\Users\khiem> wsl --import Ubuntu "E:\wsl\ubuntu" "E:\wsl\ubuntu-ex.tar"
Import in progress, this may take a few minutes.
The operation completed successfully.
PS C:\Users\khiem>
```

# install composer


```console
curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin
sudo mv /usr/local/bin/composer.phar /usr/bin/composer

```
