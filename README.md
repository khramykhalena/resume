## Храмых Алёна Дмитриевна
КНАД 242, НИУ ВШЭ  
Резюме написано на LaTeX, собирается через Docker и GitHub Actions.

https://khramykhalena.github.io/resume/resume.pdf

Автоматическая сборка PDF-резюме с помощью Docker и GitHub Actions

Как пользоваться

```bash
git clone https://github.com/khramykhalena/resume.git
cd resume
```

```bash
docker build -t resume-builder .
docker create --name resume resume-builder
docker cp resume:/cv/main.pdf ./main.pdf
docker rm resume
```
Использовала:
LaTeX + altacv.cls, Docker, GitHub Actions,Автоматизация CI/CD

