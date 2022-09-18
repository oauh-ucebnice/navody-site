# Vytvoření nového virtuálního stroje pro předmět POS

<!-- 
Kontroluj, že je tu vše...
Složka pro vytvoření stroje ve VirtualBoxu
Spusťte VirtualBox
Soubor→ Předvolby→ Obecné
Výchozí složka pro virtuální počítače
D:\vms\vase-prijmeni
Vytvořit vlastní kopii virt. pevného disku
Originály: D:\base
Zkopírujte: D:\base\Win10lab.vhd (Původní image ponechte pro další žáky!!!)
Vaše kopie bude: D:\Win10lab-prijmeni.vhd
Vytvořte ve VirtualBoxu nový virtuální stroj
(Pokud ještě nemáte... ;) )
Název: Win10Lab
OS: Windows 10 (64 bit)
Paměť: 4096 MB
Aspoň 2048 MB ;)
Méně než 50% celkové paměti.
Připojit existující pevný disk:
Vyberte svou kopii souboru s virtuálním pevným diskem, kterou jste si vytvořili v rámci bodu 2.
Nastavit Síťový most
VM → Nastavení... → Síť
Karta 1 → Připojena k:
Síťový most
-->

1. Vytvoř nový virtuální stroj&nbsp;<br />  ![Klikni na „Nový stroj“](img/pos-vm_010_novy-stroj.png)
1. Přepnutí do _expertního režimu_ &nbsp;<br />  ![Přepnutí do expertního režimu](img/pos-vm_020_expertni-rezim.png)
1. Zadej nastavení virtuálního stroje: &nbsp;<br />  ![Nastavení stroje](img/pos-vm_030_nastaveni-stroje.png)
    - Název stroje je pro tebe, na ven vidět nejde.
    - Umístění souborů stroje bude `C:\vms\prijmeni`. Zkontroluj, že na `C:\` je složka `vms`. Další složky se vytvoří samy.
    - Disk obsahuje instalaci 64bitových Windows 10.
    - Velikost paměti by měla být nejlépe aspoň 4&nbsp;GB, ale není doporučeno přiřazovat stroji více než polovinu kapacity skutečné paměti (jezdec by měl být v&nbsp;zelené zóně).
1. K&nbsp;virtuálnímu stroji připojíme připravený virtuální disk stažený na `D:\win10lab.vdi`:<br />
    ![Přiřaď virtuálnímu stroji virtuální disk](img/pos-vm_040_pridat-disk.png)
    <br />
    ![](img/pos-vm_050_pridat-disk-ktery.png)
1. Pokud na tvém počítači chybí soubor `D:\win10lab.vdi`, nebo je poškozený, zkopíruj si ho ze serveru `\\dilna`:
    <br />
    <br />**POZOR!!! Nepřipojuj soubor ze serveru, zkopíruj si ho na `D:`!!!**
    <br />
    <br />  ![Stažení vzorového stroje](img/pos-vm_055_kopie-vzoroveho.png)
1. Potvrď připojení virtuálního disku:<br /> ![Potvrzení volby virtuálního disku](img/pos-vm_060_pridat-disk-vybrat.png)
1. Vytvoř stroj:<br /> ![Potvrzení](img/pos-vm_070_potvrd.png)
1. Nastavení síťového mostu<br />
Aby počítač mohl komunikovat ve cvičné síti, je třeba ho přepnout do režimu _síťový most_!<br />
![Nastavení síťového mostu](img/pos-vm_080_sitovy-most.png)
1. Doporučené nastavení: přiřazení více jader procesoru<br /> ![](img/pos-vm_090_volitelne-procesor.png)

> **Přepoj počítač ze školní do cvičné sítě!!**
>
> Před spuštěním virtuálního stroje je třeba **přepnout počítač do cvičné sítě!!!**
> Přepoj UTP kabel do správného konektoru cvičné školní sítě!

1. Spusť virtuální stroj tlačítkem _Spustit_<br /> ![Spuštění stroje](img/pos-vm_100_spustit.png)
1. Dodatečné přepnutí síťového stroje při spuštěném stroji:<br />  ![](img/pos-vm_110_sitovy-most-dodatecne.png)
1. Volitelně: přepnutí do celoobrazovkového režimu:<br />  ![Celoobrazovkový režim](img/pos-vm_120_fullscreen.png)