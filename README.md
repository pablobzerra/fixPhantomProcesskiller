# FixPhantomProcessKill

- ADB-TERMUX:
>https://github.com/MasterDevX/Termux-ADB
>
>adb pair IP:Port code

- Instalação:
```
wget https://raw.githubusercontent.com/pablobzerra/fixPhantomProcesskiller/main/fpk_FixPhantom && mv fpk_FixPhantom $PATH/fpk && chmod +x $PATH/fpk
```

- tutorial:
>fpk [adb port]

# Info

Para os não iniciados, o PhantomProcesskiller é um novo mecanismo no Android 12 que elimina processos filho bifurcados iniciados por aplicativos se estiverem usando CPU excessiva enquanto os processos do aplicativo pai também estiverem em segundo plano. Além disso, a mudança permite apenas até 32 processos filhos
