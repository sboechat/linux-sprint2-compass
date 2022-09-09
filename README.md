# Sprint 2 - Compass.uol
Repositório da segunda atividade do estágio de DevSecOps da Compass.uol, contendo o slide de apresentação, manual de instalação do Oracle Linux e histórico de modificações dos arquivos necessários para a realização da atividade.

## Alterações na VM
<p>1.0	– Máquina virtual instalada seguindo os "Passos para a Instalação do Oracle Linux". <p>
<p>2.0	– Layout do teclado modificada para br-abnt2.<p>
<p>3.0	– Interface de rede WiFi modificada do modo NAT para o modo Bridge.<p>
<p>4.0	– Configurado IP estático 168.192.10.69.<p>
<p>5.0	– Instalação do programa FilleZilla na minha máquina real Windows para criar versionamento e explorar arquivos do servidor.<p>
<p>6.0	– Instalada uma nova máquina virtual para realizar a configuração de relação de confiança.<p>
<p>7.0	– Chave ssh RSA gerada no host cliente<p>
<p>8.0	– Chave do host cliente configurada em authorized_keys no host servidor<p>

## Relação de Confiança
<p>Para estabelecer a relação de confiança com ssh, deve ser gerada a chave do lado do cliente com o comando ssh-keygen. Com a chave gerada no arquivo id_rsa.pub do cliente, ela deve ser configurada no arquivo authorized_keys do servidor.<p>
<p>Após a configuração, o host cliente conseguirá acessar o servidor com o comando ssh pela porta 22 sem a necessidade de senha. A mesma relação pode ser feita de maneira inversa, com o servidor virando cliente e o cliente virando servidor, assim terá uma relação de confiança bidirecional entre os hosts.<p>
