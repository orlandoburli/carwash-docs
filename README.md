# Projeto CarWash

## Objetivo
O objetivo é criar uma plataforma que conecte usuários de carros com prestadores de serviço de limpeza de carros, permitindo agendar serviços e efetuar pagamentos pela plataforma.

## Atores
* Administrador da plataforma;
* Proprietários de Lava-Jatos e serviços afins;
* Proprietários de carros.

### Administrador da plataforma
* H1.1 Consultar solicitações de cadastro de empresas/lava jatos;
* H1.2 Aprovar solicitação de cadastro
* H1.3 Recusar solicitação de cadastro

### Proprietários de Lava-Jatos e serviços afins
* H2.1 Cadastrar sua empresa;
	* O proprietário pode cadastrar sua empresa, informando CNPJ, Fantasia, Razão Social, Logomarca (ver medidas padrão), e conta paypal para recebimento;
	* Neste cadastro, o proprietário deve anexar documentos da empresa e de seus sócios.
		* Documentos da Empresa:
			* Comprovante de endereço da empresa;
			* de abertura da empresa, contrato social e documentos do proprietário e sócios (RG, CPF ou carteira de motorista)
	* O sistema deve validar o CNPJ para não cadastrar repetidamente na plataforma.
* H2.2 Cadastrar pontos de atendimento;
* H2.3 Abrir agenda de atendimento (dias e horários);
* H3.3 Receber agendamentos
* H3.4 Consultar agendamentos do dia
* H3.5 Consultar histórico de faturamento/agendamentos

### Proprietários de carros
* H3.1 Cadastrar-se na plataforma
	* Opção de cadastro
		* Cadastrar-se por login social
			* Facebook
			* Google
		* Cadastrar-se com dados gerais
			* Nome, eMail, CPF, Telefone
	* Confirmar Telefone via SMS (em ambos os casos)
* H3.2 Agendar atendimento lava-jato
	* Informar características do veículo
		* Carro
			* Carro pequeno
			* Carro grande (caminhonetes e afins)
		* Moto
			* Moto pequena
			* Moto grande (acima de 500cc)
	* Informar o dia e horário que se deseja agendar
	* Listar lava-jatos disponíveis na região no dia e horário solicitados
		* Formato lista
		* Formato mapa
	* Seleciona um lava-jato
	* O sistema informa o preço para as característica do veículo informado 
		* Neste preço deve estar incluído a tarifa de 10% da plataforma
	* Seleciona a forma de pagamento (inicialmente somente paypal)
	* Efetua o pagamento e agenda a entrega do veículo ou retirada pelo prestador de serviço