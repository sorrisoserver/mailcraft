# Identidade visual — Sorriso Server Mail (nome oficial)

## Referência oficial
A arte oficial foi fornecida pelo responsável pela Sorriso Server nesta conversa em 21/10/2026. É uma marca com fundo azul-marinho escuro, símbolo de nuvem e circuitos em azul/ciano, logotipo SORRISOSERVER e slogan "TRANSFORMANDO IDEIAS EM SOLUÇÕES WEB".

**Não substituir a logo por uma versão gerada ou redesenhada sem aprovação.** A imagem JPEG original precisa ser adicionada posteriormente ao repositório como ativo de referência; por enquanto, não há ativo binário nesta branch.

## Cores iniciais (aproximadas, extraídas da referência JPEG)
- Fundo principal: `#061625`
- Azul de destaque: `#138ED2`
- Azul médio: `#107EC5`

Ajustar valores finais após aprovação de visualização no aplicativo.

## Diretrizes
1. Preservar o histórico e o código-base do MailCraft, incluindo avisos de licença e atribuição.
2. Trabalhar somente na branch `branding-sorriso-server`; alterações na `main` exigem revisão.
3. A identidade visual não deve alterar protocolos IMAP/SMTP, armazenamento de credenciais ou funcionalidades de e-mail.
4. Aplicativo Windows será o primeiro alvo de testes, sem descartar suporte a outras plataformas.
5. Nome oficial aprovado pelo responsável em 21/10/2026: **Sorriso Server Mail**.

## Primeiras tarefas
- [x] Criar branch de personalização.
- [x] Registrar identidade, nome provisório e paleta inicial.
- [ ] Adicionar o arquivo original da logo ao repositório.
- [x] Localizar os pontos principais do nome da janela e dos metadados Windows.
- [x] Atualizar nome da janela e ProductName/FileDescription/CompanyName no executável Windows.
- [ ] Mapear os demais textos, ícones e identificadores do aplicativo.
- [ ] Implementar ícones e identidade visual sem alterar o funcionamento do cliente.
- [ ] Configurar compilação automatizada para Windows.
- [ ] Validar build e realizar testes práticos antes de distribuir.

## Licenciamento
A base MailCraft declara licença `MIT OR Apache-2.0`. Preservar os avisos exigidos e verificar marcas e recursos de terceiros antes de distribuir comercialmente.

## Implementação inicial (21/10/2026)
- `apps/mailcraft/src/main.rs`: título da janela, nome usado na inicialização nativa e menu macOS atualizados para Sorriso Server Mail.
- `apps/mailcraft/build.rs`: nome do produto, descrição e empresa alterados nos recursos VERSIONINFO Windows.
- O executável, os ícones embutidos, o ID de aplicativo (`io.github.billsecond.mailcraft`) e os componentes de atualização/instalação ainda mantêm identificadores originais. **Não distribuir como versão final antes de revisar esses pontos**, especialmente atualizações automáticas, caminhos de dados e associações de arquivos.
- Compilação e testes ainda não executados; nenhuma alegação de funcionamento validado.
