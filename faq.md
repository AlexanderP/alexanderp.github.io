**How to install one package ignoring others**

As an example you don’t need all the repository packages but _clementine_ only.
It’s needed to create file `/etc/apt/preferences.d/notesalexp` containing:

	Package: *
	Pin: release o=notesalexp.org
	Pin-Priority: 200
	
	Package: clementine
	Pin: release o=notesalexp.org
	Pin-Priority: 500

Now _clementine_ will be installed from http://notesalexp.org/ the other packages from other sources.

---

**Как установить только один пакет, не затрагивая другие пакеты?**

Допустим Вам ненужны все пакеты из моего репозитория, а только _clementine_. 
Тогда создадим файл `/etc/apt/preferences.d/notesalexp` со следующим содержанием:

	Package: *
	Pin: release o=notesalexp.org
	Pin-Priority: 200
	
	Package: clementine
	Pin: release o=notesalexp.org
	Pin-Priority: 500

Теперь _clementine_ будет устанавливаться с http://notesalexp.org/, а другие пакеты с других источников.
