# Windows

Há um problema específico no Windows, devido as permissões para a pasta compartilhada.

Nesse caso, para criar o virtualenv, é necessário criá-lo em outra pasta que não a compartilhada (/vagrant). Exemplo:

```shell
cd /vagrant/src/voc
python3.4 -m venv /home/vagrant/.voc
source /home/vagrant/.voc/bin/activate
./setup.py

```