# EstacionaEDGE · Demo

**▶️ Teste a demo / Try the demo: https://nanda-jatoba.github.io/estaciona-edge-demo/**

Web app para um time ver em tempo real quais vagas de estacionamento estão livres,
chamar quem está bloqueando a saída e se organizar quando o estacionamento lota.

> Esta é uma **versão demonstrativa** com **dados fictícios**: as pessoas, salas e
> telefones são inventados, e nada do que você faz aqui é enviado para nenhum servidor.
> Recarregar a página volta ao estado inicial. Aplicativo independente, não é um
> produto oficial EDGE.

<p>
  <img src="prints/02-vagas.png" width="200" alt="Painel de vagas">
  <img src="prints/03-chamar-whatsapp.png" width="200" alt="Chamar quem está bloqueando">
  <img src="prints/05-chamado.png" width="200" alt="Aviso de chamado">
  <img src="prints/06-ranking.png" width="200" alt="Ranking de uso">
</p>

## O que dá para testar

- **Estacionar e liberar:** você entra como *Camila Ribeiro*, já estacionada no fundo da vaga 210. Libere a vaga e estacione em outra.
- **Chamar quem está na frente:** na vaga 210, toque em *Chamar Rafael para descer*. Na versão real, isso abre o WhatsApp com a mensagem pronta.
- **"Sem carro?":** em uma vaga ocupada por outra pessoa, avise que ela pode estar vazia ou assuma a vaga.
- **"Pode estar ocupada":** em uma vaga livre, use o menu **⋮** para avisar que tem um carro sem cadastro.
- **Lista de espera, ranking e sugestões:** pelos ícones de sino, troféu e lâmpada.
- **Tema claro/escuro:** pelo ícone de sol/lua.
- **Seu próprio acesso:** toque em *Sair* e entre com qualquer telefone para fazer um cadastro (fica só no seu navegador).

## Sobre o projeto

No prédio onde trabalho, a empresa tem vagas fixas, e para descobrir se alguma estava
livre era preciso rodar o estacionamento conferindo uma por uma. O EstacionaEDGE resolve
isso: cada pessoa marca a vaga ao estacionar, e todo mundo vê na hora.

**Sistema real:** JavaScript (HTML/CSS/JS sem framework), Node.js/Express e PostgreSQL;
atualizações em tempo real com Server-Sent Events; regras validadas no servidor (cada pessoa
só mexe na própria vaga, sem perda por concorrência); vagas liberadas automaticamente todo
dia; publicado em VPS com Nginx e PM2 e monitorado no Grafana.

**Esta demo:** o mesmo frontend, com o armazenamento trocado por dados fictícios em memória.

---

## English

A web app that lets a team see in real time which parking spots are free, message whoever
is blocking them in, and keep a waitlist when the garage is full. This **demo uses
fictional data** (people, rooms and phone numbers are made up) and sends nothing to any
server; reloading resets it.

**Real system stack:** vanilla JavaScript, Node.js/Express, PostgreSQL, Server-Sent Events,
server-side rule enforcement, Nginx, PM2 and Grafana.

Desenvolvido por / Built by [Maria Fernanda Jatobá](https://www.linkedin.com/in/nanda-jatoba).
