# Lern-Bericht
Michael Saugy

## Einleitung

In diesem Modul ging es darum, eine Applikation vor verschiedenen Angriffen zu schützen.

## Was habe ich gelernt?

Ich habe gelernt, wie man ein Programm von SQL-Injections schützen kann und was escaping ist.

## Beschreibung

Eine Session-Fixation ist ein Angriff, bei dem man versucht, dem Opfer eine festgelegte Session-ID unterzujubeln. Wenn das Opfer (bevorzuglich ein Administrator) sich dann unter der Session-ID einloggt, kann sich der Angreiffer mit der identischen Session-ID als Opfer anmelden. Dies kann man im Programm verhindern, indem man die Session ID möglichst oft wechselt. In Java kann man in der "web.xml"-Datei die Dauer einer Session festlegen.


So könnte ein Session-Fixation Angriff aussehen:
![image](https://user-images.githubusercontent.com/69577552/207852766-344957bd-2ae8-40ef-a73d-2583539679f0.png)

So kann man die Dauer einer Session festlegen:
![image](https://user-images.githubusercontent.com/69577552/207853261-04f5a4ac-6762-4bad-8fd1-3faf57d9bd9c.png)
*in dem web.xml file

## Verifikation

In dem Text habe ich beschrieben, was eine Session-Fixation ist und wie man seine Applikation davon schützen kann. Im Screenshot zeige ich, wie man so einen Angriff startet und der beschriebene Code-Fetzen zeigt, wie man dies in Java umsetzen kann. 

# Reflektion zum Arbeitsprozess

👍 Überlegen Sie sich jeweils etwas, was gut an Ihrer Arbeit lief; 

👎 und etwas, was nicht gut lief.

**VBV**: ✍️ Formulieren Sie davon ausgehend einen *handelbaren* Verbesserungsvorschlag.
