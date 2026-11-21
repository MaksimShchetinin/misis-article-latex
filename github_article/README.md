# Сборка научной статьи

Используйте XeLaTeX с зависимостями класса и шрифтами Times New Roman и Courier New. Запускайте из этой папки:

```sh
mkdir -p build/research
latexmk -xelatex -halt-on-error -interaction=nonstopmode -outdir=build/research article/news-stability.tex
```

Результат — `build/research/news-stability.pdf`. GitHub Actions собирает этот же исходник с Tectonic на Windows и выгружает PDF как артефакт. Перед подачей укажите подтверждённый email в команде `\misisauthor` в исходнике.
