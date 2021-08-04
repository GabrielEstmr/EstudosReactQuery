## Anotações Apresentação:

=> Fácil Instalação: Métodos + Provider no APP.TSX
=> Ferramenta Desenvolvimento Integrada: tbm apenas colocar no APP.tsx
=> Redux: client-state library (controle estado dos dados no cliente)    VS    React-Query: server-state library (controla estado dos dados nas requisições APIs)




=> Dashboard => usuários --> ver que carrega mais rápido > atuação cache

        estratégia: stale while revalidate: mostra o dado em cache (obsolento) enquanto revalida/pega informações do DB

=> Revalidate on Focus:

        quando usuário sai da página e volta: revalida dados;
        da pra controlar: quanto tempo demora pra revalidar




ReactQueryDevtools 
    => Mostra dados por chave
    => Refetch: continua dados do cache e depois substitui quando há retorno da API
    => Reset: limpa cache e faz fetch/requisição API do zero 
    => Invalidade = Refetch mas com trigger baseado em tempo/ação

    => Estados dos Dados: stale, fetching (assume como default a não ser que configure), fresh
        (mostrar no focus via Devtools)



=> Estados Requisição: Mostrar nas opções no index.tsx de users (mostrar spinners)

=> criação Hook de fetch de dados