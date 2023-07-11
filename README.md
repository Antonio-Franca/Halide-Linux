# Halide em Linux
Compilar e Executar de forma simples o Halide em linux

## Primeiros passos

- Execute os seguintes comandos

```
sudo apt update

sudo apt upgrade

sudo apt install \
                  build-essential git ninja-build \
                  clang-tools lld llvm-dev libclang-dev \
                  libpng-dev libjpeg-dev libgl-dev \
                  python3-dev python3-numpy python3-scipy python3-imageio \
                  libopenblas-dev libeigen3-dev libatlas-base-dev libjpeg9
```
- Baixe e descompacte a versão mais recente do Halide de acordo com sua máquina: 
Disponível em : https://github.com/halide/Halide/releases

- Mova o arquivo descompactado para a pasta HOME do usuário conforme o exemplo:
```
mv Halide-16.0.0-x86-64-linux ~/
```
## Próximos passos

- Escolha um local onde ficarão seus projetos

- Clone o repositorio

```
git clone https://github.com/Antonio-Franca/Halide-Linux
```
- Entre na pasta

```
cd Halide-Linux
```
- Crie as seguintes pastas 
```
mkdir build output
```

## Para executar

- Compile o arquivo:
```
make file=nome_do_arquivo
```

Obs: O nome do arquivo precisa estar sem a extensão

- Execute o arquivo usando:
```
make run
```

