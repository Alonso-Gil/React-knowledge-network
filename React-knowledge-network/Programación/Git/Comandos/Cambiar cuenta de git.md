## Configurar tu dirección de correo electrónico de confirmación en Git

Puede usar el comando `git config` para cambiar la dirección de correo electrónico asociada a las confirmaciones de Git. La dirección de correo electrónico nueva que configures será visible en cualquier confirmación futura que insertes en GitHub.com desde la línea de comandos. Cualquier confirmación que realices antes de cambiar tu dirección de correo electrónico de confirmaciones estarán todavía asociadas a tu dirección de correo electrónico anterior.

### [](https://docs.github.com/es/account-and-profile/setting-up-and-managing-your-personal-account-on-github/managing-email-preferences/setting-your-commit-email-address#setting-your-email-address-for-every-repository-on-your-computer)Configurar tu dirección de correo electrónico para cada repositorio en tu computadora

1.  Abra Git Bash.
2.  Configurar una dirección de correo electrónico en Git. Puede usar la [dirección de correo electrónico `noreply`proporcionada por GitHub](https://docs.github.com/es/articles/setting-your-commit-email-address) o cualquier dirección de correo electrónico.
    
    ```shell
    $ git config --global user.email "YOUR_EMAIL"
    ```
    
3.  Confirma que has establecido correctamente la dirección de correo electrónico en Git:
    
    ```shell
    $ git config --global user.email
    email@example.com
    ```
    
4.  Agregue la dirección de correo electrónico a su cuenta en GitHub, de modo que las confirmaciones se le atribuyan y aparezcan en el gráfico de contribuciones. Para más información, vea "[Adición de una dirección de correo electrónico a la cuenta de GitHub](https://docs.github.com/es/github/setting-up-and-managing-your-github-user-account/adding-an-email-address-to-your-github-account)".