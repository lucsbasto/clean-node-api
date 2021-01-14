[alias]
	s = !git status -s
	c = !git add --all && git commit -m
	l = !git log --pretty=format:'%C(blue) %h %C(red)%d %C(white)%s - %C(cyan)%cn, %C(green)%cr'

Criar alias para os comandos do git
git log --pretty=format:'%C(blue) %h %C(red)%d %C(white)%s - %C(cyan)%cn, %C(green)%cr'

%h = hash reduzida
%d = branch
%s = subject ou mensagem do commit
%cn = commiter name
%cr = data do commit
