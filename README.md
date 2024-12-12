# RCOM Project 2

## 1. FTP Downloader

Para testar:

```bash
$ gcc -Wall -o download clientTCP.c
$ ./download ftp://ftp.up.pt/pub/gnu/emacs/elisp-manual-21-2.8.tar.gz
$ ./download ftp://demo:password@test.rebex.net/readme.txt
$ ./download ftp://anonymous:anonymous@ftp.bit.nl/speedtest/100mb.bin
```

Notas:
- Ao compilar aparecem alguns warnings mas a aplicação compila na mesma com sucesso
- O 3º URL demora bastante tempo a fechar, mesmo depois de já ter feito o download, mas em cerca de 1 minuto (?) termina