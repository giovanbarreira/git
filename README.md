# git
Respostas das atividades do livro.



RESPOSTAS
1. O Visual Studio é um ambiente de desenvolvimento integrado (IDE) da Microsoft que permite criar, depurar, testar e implantar aplicativos para diversas plataformas, como Windows, Web, Mobile, Cloud e outros. O Visual Studio oferece recursos como editor de código, designer gráfico, depurador, gerenciador de soluções, controle de versão, ferramentas de teste, extensões e muito mais.
2. A versão 2022 do Visual Studio possui quatro edições: Community, Professional, Enterprise e Code. A edição Community é gratuita e voltada para estudantes, desenvolvedores individuais e projetos de código aberto. A edição Professional é paga e destinada a equipes pequenas que precisam de ferramentas avançadas de produtividade e colaboração. A edição Enterprise é paga e indicada para equipes de qualquer tamanho que precisam de soluções escaláveis e de alto desempenho. A edição Code é gratuita e leve, ideal para desenvolvimento web e de nuvem com suporte a diversas linguagens e plataformas.
3. O Visual Studio, o Visual Studio Code e o Blend for Visual Studio são ferramentas diferentes que atendem a diferentes necessidades dos desenvolvedores. O Visual Studio é um IDE completo e poderoso que suporta principalmente o desenvolvimento de aplicações .NET e C++. O Visual Studio Code é um editor de código leve e multiplataforma que suporta diversas linguagens e cenários de desenvolvimento, como web, nuvem, Python, Java, Node.js e outros. O Blend for Visual Studio é um componente do Visual Studio que ajuda a criar interfaces de usuário baseadas em XAML para aplicações Windows e Web. Ele oferece recursos como ferramentas gráficas, animações, comportamentos e integração com o Visual Studio.
4. O Git é uma ferramenta de controle de versão distribuído que permite gerenciar e rastrear as mudanças no código-fonte de projetos de software. O Git é gratuito e de código aberto, e possui recursos como ramificação local, áreas de preparação, fluxos de trabalho múltiplos, integração com serviços de hospedagem e outros. O Git é amplamente usado por desenvolvedores de software em todo o mundo.
5. O GitHub é uma plataforma de hospedagem de código-fonte baseada no Git que permite criar, compartilhar e colaborar em projetos de software. O GitHub oferece recursos como repositórios ilimitados, revisão de código, solicitações de pull, integração contínua, ações do GitHub, patrocinadores do GitHub, discussões do GitHub e outros. O GitHub é usado por mais de 100 milhões de desenvolvedores e organizações em todo o mundo.
6. Sim, existem outros softwares similares ao GitHub, como o GitLab, o Bitbucket, o SourceForge, o Gitea e o Azure DevOps. Esses softwares também oferecem serviços de hospedagem de código-fonte baseados no Git, com diferentes recursos e preços. Alguns deles são de código aberto e permitem hospedar os projetos em servidores próprios.
7. O Git CMD é uma ferramenta de linha de comando que permite executar os comandos do Git no Windows. O Git CMD é instalado junto com o Git for Windows, que é uma distribuição do Git adaptada para o sistema operacional Windows. O Git CMD é útil para os usuários que preferem usar o Git no modo nativo do Windows, sem depender de outras ferramentas como o Bash ou o PowerShell.
8. Sim, existem outros softwares similares ao Git CMD, como o Git Bash, o Git GUI, o TortoiseGit, o Git Extensions e o Sourcetree. Esses softwares também permitem executar os comandos do Git no Windows, mas com diferentes interfaces e funcionalidades.
9. Sim, existem ferramentas gráficas para fazer a mesma coisa que o Git CMD faz com comandos. Algumas dessas ferramentas são o Git GUI, o TortoiseGit, o Git Extensions, o Sourcetree, o GitHub Desktop e o Visual Studio. Essas ferramentas permitem realizar as operações do Git, como clonar (clone), adicionar (add), confirmar, enviar (push), receber (pull), mesclar (merge) e outras, por meio de menus, botões, caixas de diálogo e outros elementos visuais.
10. CI/CD é a abreviação de Integração Contínua e Entrega Contínua, que são práticas ágeis de desenvolvimento de software que visam automatizar o processo de construção, teste e entrega de software. O objetivo da CI/CD é detectar e corrigir problemas no código o mais cedo possível, e entregar software de forma rápida, eficiente e confiável aos usuários. A CI/CD envolve a automação e o monitoramento contínuos de todo o ciclo de vida das aplicações, incluindo as etapas de integração, entrega e implantação.
11. Versionamento semântico é um conjunto de regras e requisitos para atribuir versões de software, que tenta resolver o problema conhecido como “inferno de dependências”. O versionamento semântico usa um formato de versão X.Y.Z, onde X, Y e Z são números inteiros não negativos, e indica as mudanças no código e na API pública do software. O número X representa a versão maior, que deve ser incrementado quando houver mudanças incompatíveis na API. O número Y representa a versão menor, que deve ser incrementado quando houver adição de funcionalidades compatíveis com as versões anteriores. O número Z representa a versão de correção, que deve ser incrementado quando houver correção de falhas compatíveis com as versões anteriores.



RESPOSTAS (Executadas no Git bash ou Git-CMD)
1. Para verificar a versão do git, use:
git --version

2. Para configurar o nome de usuário global e o e-mail de usuário global, use:
git config --global user.name "Mary"
git config --global user.email "mary@abc.com"

3. Para criar quatro pastas, use:
mkdir Proj1A Proj1B Proj2 Proj3

4. Para entrar em Proj1A, inicializar o git e configurar o nome de usuário e o e-mail, use:
cd Proj1A
git init
git config user.name "Joe"
git config user.email "joe@abc.com"

5, 6, 7. Faça o mesmo para Proj1B, Proj2 e Proj3, substituindo os nomes e e-mails apropriados.

8. Para verificar se algum arquivo foi alterado em Proj2, use:
cd ../Proj2
git status

9. Para criar um projeto C# console em Proj1A, você poderá criar manualmente pelo Visual Studio conforme foi feito no livro ou se você tiver o Visual Studio Code você precisará do .NET Core SDK instalado. Em seguida, você pode usar:
cd ../Proj1A
dotnet new console

Para criar e configurar o arquivo .gitignore, você pode criar um novo arquivo chamado .gitignore e adicionar as regras de ignorar arquivos. Conforme feito no livro ou ainda via linha de comando. Por exemplo:
echo "bin/" >> .gitignore
echo "obj/" >> .gitignore

10. Para adicionar as alterações, fazer o commit e o merge, use:
git add .
git commit -m "Initial commit"

11. Para criar o branch T001 e mudar para T001 de uma só vez, use:
git checkout -b T001

12. Para mudar a linha Console.WriteLine("Hello, World!"); para Console.WriteLine("Hello"), você precisará abrir o arquivo Program.cs em um editor de texto e fazer a alteração manualmente.

13. Para salvar o arquivo Program.cs e exibir as diferenças entre T001 e master, use:
git diff master

14. Para exibir informações sobre o branch T001, use:
git branch -v

15. Para adicionar as alterações, fazer o commit e o merge, use:
git add .
git commit -m "Changed greeting"
git checkout master
git merge T001

16. Para mudar a linha Console.WriteLine("Hello"); para Console.WriteLine("Oi"), você precisará abrir o arquivo Program.cs em um editor de texto e fazer a alteração manualmente.

17. Para adicionar as alterações, fazer o commit e o merge, use:
git add .
git commit -m "Changed greeting to Portuguese"

18. Para reverter o código para Console.WriteLine("Hello"), você pode usar o comando git revert. Primeiro, encontre o hash do commit que você deseja reverter usando:
git log

Em seguida, reverta para esse commit usando:
git revert <commit-hash>

Lembre-se de substituir `<commit-hash>` pelo hash do commit que você deseja reverter. Por favor, note que esses comandos são para um ambiente Unix-like (ou para Windows usando o Git-CMD) e podem variar dependendo do seu sistema operacional e configuração. Além disso, certifique-se de estar no diretório correto ao executar esses comandos. Outro ponto é que muitos desses comando podem ser feitos em ferramentas gráficas, como o próprio Git do Visual Studio. Mas para entrevistas de emprego o ideal é desenvolver uma certa fluência nestes comandos.


