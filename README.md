# Samba Connect 

> Descrilção

Conexão e montagem de um diretório hospedado em um servidor samba.
---
<br />

 Ao clonar o repositorio, tenha certeza de que seu usuário tenha permissões de execução
 para verificar basta olhar o seu arquivo sudoers.
 
<br />

> Dependências 
 
 ``` bash
    cifs cifs-utils 
 ```
<br />

>Dica

Mova o executavel para ~/.local/bin
<br />

>Como usar

Crie uma arquivo em algum local de sua home <br/>

<b>ex: smbCredentials</b></br>

Em seguida execute __chmod 600__ no arquivo e libere o acesso ao seu usuário com  __chown user:group__

Edite o arquivo smbConnect passando seu HOST ou DDNS <br>
e passando o PATH do arquivo de credenciais

Depende de como as permissões do usuário estiver configurado, o modo de uso vai ser diferenciado


<details>
    <summary> ALL=(ALL)ALL</summary>

       shell:  sudo smbConnect folder 
   
</details>
<br />
<details>
<summary>ALL=(ALL:ALL)</summary>
    
      shell:  smbConnect folder

</details>
<br/>

__Caso não tenha colocado o arquivo no ~/.local/bin
execute o comando com ./ ou sh .__

----
> __Consulte__
<b>
 https://www.redhat.com/sysadmin/using-sudo-delegate
 https://linux.die.net/man/8/mount.cifs


