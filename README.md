🧰 Pré-requisitos

💻 Kali Linux instalado em uma VM (VirtualBox)
🌐 Conexão de rede entre host e VM (modo Bridge ou Host-Only)
🔧 SEToolkit instalado (vem por padrão no Kali)
🧪 Ambiente de teste (nunca em produção!)


🔥 Passo a Passo para Clonar o Facebook com SEToolkit
1️⃣ Abrir o Terminal no Kali Linux
Shellsudo setoolkitMostrar mais linhas
2️⃣ Aceitar os termos

Digite y para aceitar os termos de uso.

3️⃣ Escolher o tipo de ataque

Digite 1 para Social-Engineering Attacks

4️⃣ Escolher o vetor de ataque

Digite 2 para Website Attack Vectors

5️⃣ Escolher o método de ataque

Digite 3 para Credential Harvester Attack Method

6️⃣ Escolher o método de entrega

Digite 2 para Site Cloner

7️⃣ Inserir o IP da sua máquina Kali

Esse IP será usado como servidor da página falsa. Você pode descobrir com:

Shellip aMostrar mais linhas
Exemplo: 192.168.0.105
8️⃣ Inserir a URL do site a ser clonado
Shellhttps://www.facebook.comMostrar mais linhas
9️⃣ SEToolkit vai clonar o site e iniciar o servidor

A página falsa estará disponível no IP da sua Kali.
Exemplo: http://192.168.0.105


🧪 Testando o site clonado

Acesse o IP da Kali a partir de outra VM (Windows, por exemplo).
Digite usuário e senha fictícios.
As credenciais serão capturadas e exibidas no terminal do SEToolkit.


📁 Onde ficam os dados capturados?

Os dados são salvos em:

Shell/var/www/htmlMostrar mais linhas

E também aparecem em tempo real no terminal do SEToolkit.


🛡️ Dicas de Segurança para Testes

Use rede Host-Only para isolar o ambiente.
Nunca acesse o site clonado fora da VM ou em máquinas com EDR (como CrowdStrike).
Use uma VM cliente para simular o acesso.


🎉 Finalizando
Parabéns! Você criou um ambiente de teste para entender como ataques de engenharia social funcionam e como se proteger deles. Esse tipo de simulação é essencial para profissionais de segurança da informação
