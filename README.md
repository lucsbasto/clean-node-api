```
[alias]
	s = !git status -s
	c = !git add --all && git commit -m
	l = !git log --pretty=format:'%C(blue) %h %C(red)%d %C(white)%s - %C(cyan)%cn, %C(green)%cr'
  ```

Criar alias para os comandos do git

```git log --pretty=format:'%C(blue) %h %C(red) %d %C(white) %s - %C(cyan) %cn, %C(green) %cr'```

```%C(color) - cor das proximas informações```

```%h = hash reduzida```

```%d = branch```

```%s = subject ou mensagem do commit```

```%cn = committer name```

```%cr = data do commit```

Conventional Commits

chore = add new config, setup or lib
add git-commit-msg-linter 

```
git c "add commit linter"

************* Invalid Git Commit Message **************
  commit message: add commit linter
  correct format: <type>(<scope>): <subject>
  example: docs: update README add developer tips

  type:
    feat     A new feature
    fix      A bug fix
    docs     Documentation only changes
    style    Changes that do not affect the meaning of the code (white-space, formatting, missing semi-colons, etc)
    refactor A code change that neither fixes a bug nor adds a feature
    test     Adding missing tests or correcting existing ones
    chore    Changes to the build process or auxiliary tools and libraries such as documentation generation
    perf     A code change that improves performance
    ci       Changes to your CI configuration files and scripts
    build    Changes that affect the build system or external dependencies (example scopes: gulp, broccoli, npm)
    temp     Temporary commit that won't be included in your CHANGELOG

  scope:
    Optional, can be anything specifying the scope of the commit change.
    For example $location, $browser, $compile, $rootScope, ngHref, ngClick, ngView, etc.
    In App Development, scope can be a page, a module or a component.

  subject:
    Brief summary of the change in present tense. Not capitalized. No period at the end.```