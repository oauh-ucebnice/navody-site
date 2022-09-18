# Povolení služby „PING“ ve firewallu

> Poznámka: Jedná se o službu _echo_ protokolu ICMP. Lidově se nazývá „PING“.

## Postup (česká Windows):
1. _Start_ → _Firewall v programu Windows Defender_
2. _Upřesnit nastavení_ → _Příchozí pravidla_
3. Povolte pro všechny typy sítí pravidla:<br />
    - _Sdílení souborů a tiskáren (Požadavek na odezvu - ICMPv4-In)_
    - _Zjištění stavu virtuálního stroje (Požadavek na odezvu - ICMPv4-In)_
4. Vpravo zelená šipka „Povolit pravidlo“

## Postup (anglická Windows):
1. _Start_ → _Firewall v programu Windows Defender_
2. _Advanced Settings_ → _Inbound rules_
3. Povolte pro všechny typy sítí pravidla:<br />
    - _File and Printer Sharing (Echo Request - ICMPv4-In)_
    - _... (Echo Request - ICMPv4-In)_
4. Vpravo zelená šipka „Povolit pravidlo“

> **Pokud PING zlobí, zkuste dočasně zakázat firewall!!!** Až bude „PING“ fungovat bez firewallu, zkuste ho znovu povolit.