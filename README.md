# O que é HACS?

É uma abreviação de “Home Assistant Community Store” ou simplesmente a loja da comunidade do Home Assistant.

Sempre que desejamos utilizar projetos em uma interface com componentes customizados. Como um botão, gráficos diferentes, com linhas mais atraentes, ou com barras, cartões personalizados, temas para o HA, etc. Para poder personalizar as telas do  HA como os exemplos citados, é necessário a instalação de componentes customizados.

Antes da existência do HACS, todo componente era instalado manualmente. Agora com o HACS, o usuário utiliza de uma interface gráfica para lidar com downloads de necessidades personalizadas.

As principais vantagens do HACS são:

* Descobrir novos elementos personalizados;
* Auxilia a instalar (download) novos elementos personalizados;
* Auxilia o acompanhamento das atualizações seus elementos personalizados;
* Gerenciamento destes componentes (Instalar / Atualizar / Remover);
* Cria atalhos para repositórios / rastreador de problemas;


## Requisitos

- Você está executando a versão 2022.11.0 ou mais recente do Home Assistant.
- Você possui uma instalação suportada do Home Assistant.
- Você tem a [my integration](https://www.home-assistant.io/integrations/my/) habilitada.
- Você tem acesso ao sistema de arquivos onde os arquivos de configuração do Home Assistant estão localizados.
- Você sabe como acessar o arquivo de log do Home Assistant.
- Você está ciente de que não existem add-ons no HACS.
- Você possui uma conexão de internet estável com dados disponíveis suficientes ou sem limite de dados.

## Download

1. Acesse a loja de Add-ons.

2. Instale um dos Add-ons SSH (você precisa habilitar o modo avançado no seu perfil de usuário para vê-los).

3. Configure o Add-on SSH que você escolheu seguindo a documentação correspondente.

4. Inicie o Add-on SSH.

5. Conecte-se ao Add-on SSH.

6. Execute o script de download do HACS

   ```bash
   wget -O - https://get.hacs.xyz | bash -
   ```

## Configuração

1. Na interface do usuário do Home Assistant, vá para o painel de Integrações.
2. Limpe o cache do seu navegador. Antes que o HACS possa aparecer na lista, você precisa limpar o cache do seu navegador ou realizar uma atualização forçada.
3. Clique no botão "+ ADICIONAR INTEGRAÇÃO" no canto inferior direito.
4. Pesquise ou role para baixo até encontrar "HACS" e selecione-o.

   ![imagem](https://hacs.xyz/assets/images/conf3-6e4410a69b3429e2f3511562b1ebfb44.png)

5. Aceite os termos de uso. Nenhum dos itens é opcional, você precisa aceitar tudo antes de poder configurar o HACS.

   ![imagem](https://hacs.xyz/assets/images/part1-3f4090241cb4dc5c13c326c722fdb270.png)

6. Registro do dispositivo. O HACS utiliza um fluxo de autenticação de dispositivo OAuth para se autenticar na API do GitHub. Na primeira tela, você verá um código de dispositivo, copie-o para a área de transferência e clique no link [https://github.com/login/device](https://github.com/login/device) para continuar a configuração. **Não clique em enviar ainda!**

   ![imagem](https://hacs.xyz/assets/images/part2-2f7d42ee3716a19820977439e24f6973.png)

7. Se você não estiver conectado ao GitHub no seu navegador, será necessário se cadastrar ou entrar para continuar a configuração. Se você já estiver conectado, pode pular esta parte.

   ![imagem](https://hacs.xyz/assets/images/no_account-c5267b04716e84b787cbc046df5c1123.png)

8. Quando a página for carregada, cole ou digite o código de dispositivo que foi apresentado na etapa anterior.

   ![imagem](https://hacs.xyz/assets/images/part3-a1c5286f5f21118023870275fb448370.png)

9. Clique em "Autorizar hacs".

   ![imagem](https://hacs.xyz/assets/images/part4-6f36bdc5a6cc418197915f78356eee9f.png)

10. Quando você visualizar a tela de confirmação, pode fechar a aba e voltar para o Home Assistant.

    ![imagem](https://hacs.xyz/assets/images/part5-f1bdc86cafaac28b0325fe2981bb599f.png)

11. Agora você pode clicar em "Enviar" para concluir a configuração do HACS.

    ![imagem](https://hacs.xyz/assets/images/part2-2f7d42ee3716a19820977439e24f6973.png)

12. Se tudo correr bem, verá a tela "Sucesso". Clique em Terminar.

## Instalando Integrações Personalizadas e Temas Usando o HACS

Após instalar e configurar o HACS com sucesso, você pode usar a community store para buscar e instalar integrações personalizadas e temas. Os passos são os seguintes:

1. Clique na opção HACS na barra lateral e, em seguida, clique em Integrações.

2. Clique no botão Explorar e Baixar Repositórios.

3. Procure pela integração que você deseja instalar.

4. Assim que encontrar a integração desejada, clique nela e depois no botão Baixar.

5. Após o download da integração, vá para Ferramentas de Desenvolvedor e clique em Reiniciar. É necessário reiniciar o servidor do Home Assistant para que as alterações tenham efeito.

6. Da mesma forma, você pode clicar em HACS > Frontend para encontrar e instalar temas personalizados e cartões para personalizar a aparência do painel do seu Home Assistant, interruptores e entidades.
