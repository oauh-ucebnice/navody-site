# Povolení služby „PING“ ve firewallu

> Poznámka: Jedná se o službu _echo_ protokolu ICMP. Lidově se nazývá „PING“.

> **Pokud PING zlobí, můžete zkusit dočasně zakázat firewall!** Až opravíte nastavení a až bude „PING“ fungovat bez firewallu, firewall znovu povolte.

## Postup (česká Windows):
1. _Start_ → _Firewall v programu Windows Defender_
2. _Upřesnit nastavení_
3. _Příchozí pravidla_
4. Povolte pro všechny typy sítí pravidla:<br />
    - _Sdílení souborů a tiskáren (Požadavek na odezvu - ICMPv4-In)_
    - _Zjištění stavu virtuálního stroje (Požadavek na odezvu - ICMPv4-In)_
5. Vpravo zelená šipka „Povolit pravidlo“

Postup (screenshoty):
1. <br />![Start → Firewall](img/pos-firewall_010_start.png)
2. <br />![Upřesnit nastavení → Příchozí pravidla](img/pos-firewall_020_upresnit.png)
3. <br />![Start → Povolit ICMPv4-In](img/pos-firewall_030_povolit.png)

## Postup (anglická Windows):
1. _Start_ → _Firewall v programu Windows Defender_
2. _Advanced Settings_ → _Inbound rules_
3. Povolte pro všechny typy sítí pravidla:<br />
    - _File and Printer Sharing (Echo Request - ICMPv4-In)_
    - _... (Echo Request - ICMPv4-In)_
4. Vpravo zelená šipka „Povolit pravidlo“
