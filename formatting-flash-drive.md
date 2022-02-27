# Formatando um pendrive

1. Abra o **CMD**, **PowerShell**, **Windows Terminal**, **Git Bash** ou **qualquer outro terminal**.
2. Entre no DISKPART, digitando: 

```bash
diskpart
```

3. Liste os discos disponíveis, digitando: 

```bash
list disk
```

4. Selecione o disco que você deseja formatar, digitando:

```bash
select disk 1
## Digite o número correspondente ao disco desejado. Observe o tamanho do volume do disco.
```

5. Limpe o disco, digitando:

```bash
clean
```

6. Crie uma partição primária, digitando:

```bash
create partition primary
```

7. Formate o pendrive no sistema de arquivos desejado, digitando:

```bash
format fs=fat32 quick
## Caso queira o sistema NFTS basta digitar 'nfts' no lugar de 'fat32'.
## Caso não queira uma formatação rápida, basta omitir a palavra quick, a formatação vai demorar mais.
```

8. Ative o pendrive, digitando:

```bash
active
```

9. Atribua automaticamente uma letra de unidade para que ela fique visível no Explorar de Arquivos, digitando:

```bash
assign
```

10. Saia do DISKPART, digitando:

```bash
exit
```

(Opcional) Saia do terminal, digitando novamente:

```bash
exit
```