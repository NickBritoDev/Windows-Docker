# Windows + Docker 🐋🪟

Instalar Alpine WSL:

[Alpine WSL - Aplicativo oficial na Microsoft Store](https://apps.microsoft.com/detail/9P804CRF0395?hl=pt-br&gl=BR)

Instalar o Docker:

[Get Started | Docker](https://www.docker.com/get-started/)

Terminal WSL(alpine)
Adcione a Libstdc++:

Ela fornece implementações de classes e funções padrão da linguagem C++, como contêineres, algoritmos e manipulação de strings. (extremamente necessario para manipulação dos contêineres no docker )

```bash
su
```

```bash
 apk update
```

```bash
 apk add libstdc++
```

Adicione MakeFile:

O Makefile e a ferramenta **`make`** são usados para automatizar o processo de compilação e construção de programas a partir do código-fonte. 

```bash
su
apk add make
```

Adicione o Git:
O Git é um sistema de controle de versão distribuído amplamente utilizado para rastrear alterações em projetos de software.

```bash
su
apk add git
```

Ativar uso de wsl no docker:

1. Abra o Docker Desktop no seu Windows 11.
2. Vá para as configurações do Docker Desktop.
3. Vá para a seção "General".
4. Marque a opção "Use the WSL 2 based engine".

Crie um arquivo Makefile:

```makefile
.PHONY: up
up:
	    docker run hello-world
```

Abra o terminal do projeto no alpine(wsl)

Teste conexão do docker:

```bash
make up
```
