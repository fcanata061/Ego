# Ego – Gerenciador de Pacotes Source-Based

![Ego Logo](docs/logo.png) <!-- opcional: adicione um logo -->

Ego é um **gerenciador de pacotes Linux source-based**, inspirado em Portage e PKGBUILD, que permite compilar, instalar e gerenciar programas diretamente do código-fonte. Ele resolve dependências automaticamente, aplica patches, empacota programas e permite manter um repositório local ou remoto.

---

## 🌟 Recursos Principais

- Compilação e instalação de pacotes a partir do código-fonte
- Resolução automática de dependências
- Aplicação automática de patches
- Empacotamento com `DESTDIR` e `fakeroot`
- Suporte a hooks antes/depois de cada etapa
- Logging completo e SHA256 para integridade
- Rebuild completo do sistema (`world`)
- Suporte a flags: `--force`, `--upgrade`, `--sync`, `--world`

---

## 🛠️ Instalação

### Pré-requisitos

- Bash 5+
- Make, GCC, Binutils
- Curl, Wget, Git
- Python 3
- Ferramentas de descompactação: tar, unzip, xz, bzip2

### Instalação

``` bash
# Clonar o repositório
git clone https://github.com/seuusuario/ego.git /opt/ego

# Instalar
cd /opt/ego
make install

# Adicionar ao PATH
export PATH=/opt/ego/bin:$PATH
```
