# Como Criar a Imagem e o Contêiner Docker

## Pré-requisitos

- Docker instalado na máquina. [Instruções de instalação](https://docs.docker.com/get-docker/).
- No caso, o professor sugeriu a utilização de uma máquina virtual Linux - Ubuntu.

---

## Passos para Criar a Imagem e o Contêiner

1. **Clone o repositório:**
   ```bash
   git clone https://github.com/VitorCaue/Docker-Pos
   cd Docker-Pos

2. **Crie a imagem Docker:**

```bash
 docker build -t vitorcaue03ads/docker-pos:1.0.0 .

3. **Execute o contêiner:**

```bash
docker run -d -p 80:80 vitorcaue03ads/docker-pos:1.0.0

4. **Acesse a aplicação:**
Abrir o navegador usando o ip da maquina virtual ou usando "localhost:8080" no navegador


### Passos para Publicar a Imagem

1. **Crie uma conta no Docker Hub:**  
   - Acesse Docker Hub(https://hub.docker.com/) e crie uma conta caso ainda não tenha uma.

2. **Faça login no Docker Hub pelo terminal:**
   ```sh
   docker login
   ```
   - Insira seu nome de usuário e senha do Docker Hub.
   
3. **Envie a imagem para o Docker Hub:**
   ```sh
   docker push vitorcaue03ads/docker-pos:1.0.0
   ```

---
