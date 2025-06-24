📝 Автоматическая сборка PDF-резюме с помощью Docker и GitHub Actions

Как пользоваться

```bash
git clone https://github.com/khramykhalena/resume.git
cd latex-resume
```

```bash
docker build -t resume-builder .
docker create --name resume resume-builder
docker cp resume:/cv/main.pdf ./main.pdf
docker rm resume
```
Использовала:
LaTeX + altacv.cls, Docker, GitHub Actions,Автоматизация CI/CD
