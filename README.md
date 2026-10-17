<div align="center">

<img src="assets/chuva.svg" alt="0r4y — Python · SQLite3 · Discord bots" width="100%">

<br>

<img src="https://img.shields.io/badge/Python-0b1220?style=for-the-badge&logo=python&logoColor=9fc4ff" alt="Python">
<img src="https://img.shields.io/badge/SQLite3-0b1220?style=for-the-badge&logo=sqlite&logoColor=9fc4ff" alt="SQLite3">
<img src="https://img.shields.io/badge/discord.py-0b1220?style=for-the-badge&logo=discord&logoColor=9fc4ff" alt="discord.py">
<img src="https://img.shields.io/badge/Git-0b1220?style=for-the-badge&logo=git&logoColor=9fc4ff" alt="Git">

</div>

<br>

```python
import sqlite3

conn = sqlite3.connect("0r4y.db")
conn.execute("CREATE TABLE IF NOT EXISTS sobre (chave TEXT PRIMARY KEY, valor TEXT)")
conn.executemany("INSERT OR REPLACE INTO sobre VALUES (?, ?)", [
    ("usuario",   "0r4y"),
    ("linguagem", "Python"),
    ("banco",     "SQLite3"),
    ("faz",       "bots para Discord"),
    ("clima",     "chuvoso ☔"),
])

for chave, valor in conn.execute("SELECT * FROM sobre"):
    print(f"{chave:>10} → {valor}")
```

<br>

### ☔ Projeto em destaque

<table>
  <tr>
    <td>
      <a href="https://github.com/0r4y/Bot-discord"><b>🕯️ Bot-discord</b></a><br>
      <sub>Bot de comunidade para Discord em Python: moderação, tickets, sorteios, logs, boas-vindas
      e uma sociedade secreta com credenciais e GIFs gerados na hora.</sub><br><br>
      <code>python</code> <code>discord.py</code> <code>sqlite3</code>
    </td>
  </tr>
</table>

<br>

<img src="assets/chuva-rodape.svg" alt="" width="100%">
