# Trust me

## First

Бывает текст _курсивом_, **полужирным** и ~~зачеркнутым~~  
Вот так выглядит код:

```
git add --all
git commit -m "<message>"
git push -u origin master
```

---
Хеш - уникальный идентификатор коммита

Лог - история коммитов

HEAD - файл, указывающий на последний коммит
---
Статусы:
1. untracked
2. staged
3. modified
4. tracked

```mermaid
flowchart TD
	A[untracked] -- git add --> B[staged + tracked];
	B -- change --> C[modified];
	C -- git add --> B;
	B -- git commit --> D[tracked];
	D -- change --> C;
```

---
Сообщения к коммитам указываются с инфинитивом в начале.