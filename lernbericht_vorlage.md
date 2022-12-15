# Lern-Bericht
Michael Saugy

## Einleitung

In diesem Auftrag ging es um das Schützen einer Applikation von Session-Fixation Angriffen.

## Was habe ich gelernt?

Ich habe gelernt, was eine Session-Fixation ist und wie man seine Applikation besser davor schützen kann.

## Beschreibung

Eine Session-Fixation ist ein Angriff, bei dem man versucht, dem Opfer eine festgelegte Session-ID unterzujubeln. Wenn das Opfer (bevorzuglich ein Administrator) sich dann unter der Session-ID einloggt, kann sich der Angreiffer mit der identischen Session-ID als Opfer anmelden. Dies kann man im Programm verhindern, indem man die Session ID möglichst oft wechselt. In Java kann man in der "web.xml"-Datei die Dauer einer Session festlegen.


So könnte ein Session-Fixation Angriff aussehen:
![image](https://user-images.githubusercontent.com/69577552/207852766-344957bd-2ae8-40ef-a73d-2583539679f0.png)

So kann man die Dauer einer Session festlegen:
```
<session-config>
        <session-timeout>30</session-timeout> <!--Gibt an, wielange eine Session gültig ist-->
        <cookie-config>
        <http-only>true</http-only>
        </cookie-config>
        <tracking-mode>COOKIE</tracking-mode>
</session-config>
```
*in dem web.xml file

## Verifikation

In dem Text habe ich beschrieben, was eine Session-Fixation ist und wie man seine Applikation davon schützen kann. Im Screenshot zeige ich, wie man so ein Angriff aussehen könnte und der beschriebene Code-Fetzen zeigt, wie man dies in Java umsetzen kann. 

# Reflektion zum Arbeitsprozess

Positiv:
Als ich verstanden habe, was eine Session-Fixation ist und was man damit erreicht kann, konnte ich den Auftrag sehr schnell lösen.

Negativ:
Leider hatte ich zu Beginn starke verständniss Probleme mit der Session-Fixation. Ich habe nicht verstanden, was man damit erreichen konnte oder wie man eine Session-Fixation durchführt.


**VBV**:
Da ich wie bereits erwähnt zu Beginn verständniss Probleme hatte, werde ich bei der nächsten Aufgabe früher nach Hilfe fragen. Somit hätte ich mir sehr viel Zeit und Aufwand ersparen können.
