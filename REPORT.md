# Лабораторная работа 2. Ветвление

### $ git branch
  feature-a
  feature-b
* master

### $ git branch -v
  feature-a cae4a66 feature-a: правка app.txt
  feature-b 72068cd feature-b: добавлен b.txt
* master    ebb48a5 master: добавлен m.txt

### $ git log --oneline --graph --all --decorate
* cae4a66 (feature-a) feature-a: правка app.txt
* e8bd08e feature-a: добавлен a.txt
| * 72068cd (feature-b) feature-b: добавлен b.txt
|/  
| * ebb48a5 (HEAD -> master) master: добавлен m.txt
|/  
* f10e97b base

### $ git diff master feature-a --stat
 a.txt   | 1 +
 app.txt | 1 +
 m.txt   | 1 -
 3 files changed, 2 insertions(+), 1 deletion(-)

### $ git diff feature-a feature-b --stat
 a.txt   | 1 -
 app.txt | 1 -
 b.txt   | 1 +
 3 files changed, 1 insertion(+), 2 deletions(-)
