# Análise e previsão de autorizações utilizando modelos preditivos
Trabalho de Conclusão de Curso apresentado ao Curso de Especialização em Ciência de Dados e Big Data



A autorização é um dos diversos mecanismos utilizados pelas operadoras de planos de saúde visando controlar o uso ou a demanda de serviços prestados aos beneficiários. Nesse cenário, uma autorização prévia para realizar exames e processos de alta complexidade é um dos mecanismos das operadoras para gerenciar a utilização dos seus serviços. 

Outras maneiras de controle incluem o direcionamento, (que encaminha exames, internações e consultas para a rede credenciada) e a coparticipação (em que o cliente paga uma parcela da despesa do seu procedimento). Há ainda a franquia, na qual um valor máximo para procedimentos é definido em contrato. Se o procedimento extrapolar esse teto, o plano de saúde não tem responsabilidade sobre a cobertura.

Ao controlar melhor as demandas dos serviços prestados aos seus beneficiários, as operadoras conseguem promover um uso mais consciente de seus benefícios. Dessa forma, é possível evitar o desperdício de recursos e a sobrecarga no sistema.

É importante lembrar, ainda que, a autorização no plano de saúde e outros mecanismos de regulação devem ser primeiramente analisados, a Agência Nacional de Saúde Suplementar (ANS), que é a agência reguladora vinculada ao Ministério da Saúde do Brasil, que regula o mercado de planos privados de saúde por determinação da Lei nº 9.656 de 3 de junho de 1998. A condição do órgão para a liberação desses mecanismos é que eles não impeçam ou dificultem o acesso dos usuários aos procedimentos que estão presentes no contrato do plano.

O processo para solicitar a autorização costuma variar de acordo com o plano e o tipo do procedimento. A autorização para exames, internações e serviços específicos costuma envolver a ida até a rede credenciada mais próxima com a guia ou pedido médico do exame/procedimento, o cartão de identificação do plano e um documento pessoal (como o RG). Algumas operadoras também trabalham com solicitações via internet.



O projeto tem como objetivo propor um modelo preditivo para previsão das situações das autorizações solicitas a operadora de plano de saúde, utilizando informações das autorizações já analisadas pelos auditores.

Justificativa<br>
O processo atual de autorização de procedimentos ocorre da seguinte forma. Alguns procedimentos realizados pelos beneficiários sejam eles consultas, exames ou cirurgias, geram pedidos de autorização junto a operadora. Esse pedido é chamado guia de autorização, essas guias são recebidas de forma eletrônica e na forma física. Alguns desses procedimentos são autorizados de forma automática pois no sistema de gestão da operadora existem regras configuradas que determinam se o procedimento vai ser autorizado automaticamente ou se será necessário a validação de um auditor.
O auditor é o médico responsável por analisar a guia e decidir se será autorizada ou negada. Para tomar essa decisão o médico usa de várias informações como, histórico médico do paciente, informações sobre os tipos de serviços, os valores dos itens solicitados e resoluções da ANS. 
Todo o processo de auditoria exige precisão e agilidade, pois são procedimentos que podem primeiramente salvam vidas, e que também afetam diretamente a saúde financeira da operadora caso a análise não seja feita da forma correta.
Como o volume de solicitações é elevado e carecem de uma análise profunda de auditoria, o processo geralmente é caro e pouco assertivo. Diante disso propõe-se um modelo preditivo baseado no histórico de auditoria capaz prever se a solicitação será autorizada ou negada.

Fontes de dados<br>
Os dados utilizados são privados e vieram de uma fonte principal que é o data warehouse (DW) da operadora, onde se encontra centralizado informações de diversos sistemas que são utilizados pela empresa.

Objetivo da análise<br>
O objetivo é analisar as características das autorizações auditadas e propor um modelo preditivo usando seus principais atributos para classificá-las em autorizada ou negada.



