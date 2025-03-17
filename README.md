# Configuração de Pesquisa de IA com Azure

Este `README.md` fornece um passo a passo para configurar uma pesquisa utilizando Azure AI Search e Azure AI Services, utilizando um Azure Storage para a importação de dados. Além disso, inclui insights obtidos durante o processo, ferramentas que podem se beneficiar dessa configuração e os aprendizados adquiridos. Para mais detalhes, consulte [este link](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/11-ai-search.html).

## Passo a Passo para Configuração

1. **Criação do Serviço Azure Cognitive Search**

   - Acesse o [portal do Azure](https://portal.azure.com/).
   - Clique em "Criar um recurso" e procure por "Azure Cognitive Search".
   - Selecione "Azure Cognitive Search" e clique em "Criar".
   - Preencha as informações necessárias, como Nome, Região e Grupo de Recursos.
   - Clique em "Revisar + criar" e depois em "Criar".

2. **Configuração do Azure Storage**

   - No portal do Azure, crie uma conta de armazenamento (Storage Account).
   - Navegue até a conta de armazenamento criada e clique em "Containers" para criar um novo contêiner onde os dados serão armazenados.
   - Faça upload dos arquivos de dados para o contêiner criado.

3. **Configuração do Azure AI Services**

   - Navegue para "Criar um recurso" e procure por "Azure AI Services".
   - Selecione "Azure AI Services" e clique em "Criar".
   - Preencha as informações necessárias e finalize a criação do recurso.

4. **Configuração do Índice de Pesquisa**

   - Após a criação do serviço de pesquisa, vá para a página do serviço de pesquisa.
   - Na barra lateral esquerda, clique em "Índices" e depois em "Criar índice".
   - Defina o nome do índice e configure os campos necessários (por exemplo, ID, Título, Conteúdo).
   - Clique em "OK" para criar o índice.

5. **Importação de Dados do Azure Storage**

   - Na página do serviço de pesquisa, clique em "Importar dados".
   - Selecione "Azure Blob Storage" como a fonte de dados.
   - Configure a conexão com o Azure Storage utilizando a cadeia de conexão (connection string) da conta de armazenamento.
   - Mapeie os campos dos arquivos de dados para os campos do índice.
   - Clique em "OK" para importar os dados.

6. **Configuração do Indexador**

   - Na página do serviço de pesquisa, clique em "Indexadores" e depois em "Criar indexador".
   - Defina o nome do indexador e configure a frequência de indexação.
   - Selecione o Azure Blob Storage como a fonte de dados e o índice de destino.
   - Clique em "OK" para criar o indexador.

7. **Testando a Pesquisa no Portal do Azure**

   - Na página do serviço de pesquisa, clique em "Explorar dados".
   - Selecione o índice criado e faça consultas utilizando a interface do portal.
   - Visualize os resultados e ajuste as consultas conforme necessário.

## Insights Obtidos

- **Precisão dos Resultados**: A precisão dos resultados de pesquisa depende muito da configuração do índice e da qualidade dos dados importados.
- **Flexibilidade**: O Azure Cognitive Search permite a configuração de indexadores e a importação de dados de diversas fontes, proporcionando flexibilidade na criação de soluções de busca.
- **Facilidade de Uso**: A interface do portal do Azure facilita a configuração e o teste de serviços de pesquisa sem a necessidade de codificação.

## Ferramentas que se Beneficiam

- **Motores de Busca Personalizados**: Ferramentas que oferecem buscas personalizadas em sites específicos.
- **Assistentes Virtuais**: Assistentes que necessitam buscar informações na web para responder perguntas dos usuários.
- **Sistemas de Recomendação**: Sistemas que recomendam conteúdos baseados em buscas realizadas pelos usuários.

## Aprendizados Adquiridos

- **Configuração de Serviços de IA**: Aprendizado sobre como configurar e integrar serviços de pesquisa do Azure.
- **Importação e Indexação de Dados**: Entendimento sobre a importância da configuração correta de fontes de dados e indexadores.
- **Utilização da Interface do Portal do Azure**: Experiência prática na utilização da interface do portal do Azure para configurar e testar serviços de pesquisa.

## Conclusão

A configuração de uma pesquisa utilizando IA na plataforma Azure pode ser extremamente benéfica para diversas aplicações, desde motores de busca personalizados até assistentes virtuais. O processo requer atenção na configuração dos serviços e na qualidade dos dados importados para garantir a relevância dos resultados.

Para mais detalhes, consulte [este link](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/11-ai-search.html).
