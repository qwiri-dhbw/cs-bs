## Virtuelle Adressierung

> **Beschreiben Sie die einstufige virtuelle Adressierung.**
>
> b) Welche Bedeutung haben die Einträge in der Page-Tabelle?

ANSWER

---

> **In einem 32-Bit-System mit `4kB` großen Seiten wird die zweistufige virtuelle Adressierung eingesetzt.**
> 
> a) Wie viele Speicher und wie viele Tabellen braucht man mindestens für die Speichertabellen (PD, PT)
> eines kleinen Programms (mit Code, Date, Heap und Stack)?
> 
> b) Wozu dient der TLB?
> 
> c) Für welche Bereiche des virtuellen Adressraums werden diese benötigt?

---

> **Virtuelle Adressierung bei 32-Bit mit `4MB` Seiten.**
>
> a) Wie wird die Virtuelle Adresse aufgeteilt (quantitativ)?
>
> b) Wie "berechnet" die MMU dabei die reelle Adresse (Zeichnung)?
>
> c) Wie wird durch die virtuelle Adressierung verhindert, dass Programme auf fremden Adressraum zugreifen?

---

> ![](./assets/SCR-20230618-ohri.png)
> 
> a) Beschreiben Sie, wie die reelle Adresse gebildet wird
>
> b) Wie groß sind die Register?
>
> c) Warum ist diese Tabellengröße gewählt? Was kann man tun, um größere Seiten hinzubekommen?

---

> **Gegeben sei die virtuelle Adresse `0x5678` und der Anfang der Page-Tabelle (Einstufige Adressumsetzung, Seitengröße `4kB`)**
>
> a) Ermitteln Sie die reelle Adresse im Hauptspeicher
>
> b) Was geschieht, wenn dort ein Wert eingetragen wird?

---

> a) Beschreiben Sie die Funktionsweise der virtuellen Adressierung eines 32-Bit-Prozessors mit einer Seitengröße von 4MB
>
> b) Wie vermeidet man, dass bei jeder Speicheradressierung die vollständige Adressumsetzung erfolgen muss?

---

> a) Warum wird die einstufige virtuelle Adressierung nicht verwendet?
>
> b) Wie arbeitet die virtuelle Adressierung tatsächlich?

---

> Was ist eine IOMMU? Und wofür wird sie verwendet?

ANSWER

---






## Dateisysteme

> Funktionsweise ext4

ANSWER

---

> Funktionsweise ext2

ANSWER

---

> Funktionsweise FAT

ANSWER

---

> [ext4] Beschreiben Sie den Aufbau des Dateisystems `ext4`

ANSWER

---

> [ext4] Beschreiben Sie die Funktionsweise des ext4-Dateisystems mit Extents

ANSWER

---

> [ext4] Warum kann ext4 mit Extents größere Partitionen verwalten als ohne Extents

ANSWER

---

> [ext4] Wie groß kann eine Datei werden (Blockgröße 4kB, Rechenweg)

ANSWER

---

> **Gegeben sei ein ext2-Dateisystem mit einer Blockgröße von `4kB`. Im Dateikopf seien 12 Einträge für die direkte Adressierung von Datenblöcken und 3 Einträge für die Verweise auf 1 bis 3-fach indizierte Blöcke.**
>
> a) Wie groß kann eine Datei werden (Berechnungsformel)
>
> b) Wie groß kann eine Datei werden für Blockgröße 1kB

---

> **Gegeben sei ein ext2-Dateisystem mit Blockgröße von `1kB`, 10 Einträge für direkte Adressierung, 3 Einträge für 1 bis 2-fache Adressierung.**
>
> a) Wie kann man aus den Einträgen erkennen, in welchen Blöcken die Daten gespeichert sind (Zeichnung)? 
>
> b) Maximale Dateigröße?

---

M2021

> ![](./assets/SCR-20230618-ohjd.png)
> 
> **Ein Dateisystem sei wie im Bild aufgebaut. Die Blockgröße sei `1kB`.**
>
> a) Was stellt die linke Grafik dar, was die rechte?
>
> b) Wie lange ist die Datei (erste Zeile) maximal?
>
> c) Um welches Dateisystem handelt es sich?
>
> d) Welche Aufgabe fehlt, um die genaue Dateigröße zu bestimmen?

---








## Prozesskommunikation

2022

> Wie kann der Empfänger vom Senden der Nachricht informiert werden, wenn er nicht dauernd nachfragen will?

ANSWER

---

> **Ein Prozess möchte einem anderen Prozess Nachrichtenblöcke variabler Länge schicken. Der Empfänger möchte die Nachricht mit einem Aufruf lesen, ohne die Länge der Nachrichten zu kennen.**
>
> Welches Kommunikationsmittel sollte man dafür verwenden?

ANSWER

---

> Vergleichen Sie die Eigenschaften von Pipes und Message-Queues

ANSWER

---

> a) Was sind Signale?
>
> b) Wie werden sie behandelt?

ANSWER

---

> Warum kann man einzelne Signale nicht überladen?

ANSWER

---

> Warum kann man Signale überladen?

ANSWER

---

> Was ist ein Semaphor? Wie wird er verwendet?

ANSWER

---













## Prozesse

> **Was ist ein Prozess?**
>
> b) Welche Zustände kann er einnehmen?
>
> c) Wie gelangt er von einem Zustand in einen anderen?

---

> Erklären Sie Multilevel Feedback Scheduling

ANSWER

---

> Nennen Sie 2 Gründe/Vorteile, weshalb diese Methode eingesetzt wird

ANSWER

---

> Was ist ein Thread?

ANSWER

---

> Wie verhalten sich Prozesse gegenüber Threads?

ANSWER

---

> Was sind KLTs, was sind ULTs?

ANSWER

---

> Zeigen Sie die Speicherbelegung von Threads

ANSWER

---

> Welcher Typ von Threads kann ein Mehrprozessorsystem nutzen? Warum?

ANSWER

---

> Sie haben mehrere Threads, die ihre Ergebnisse in einer gemeinsamen Variable aufsummieren.
> Können Sie, da die Addition kommutativ ist, auf kritische Bereiche verzichten?
> Wenn nein, wie würden Sie das Problem lösen?

ANSWER

---

> a) Was sind Memory Mapped Files?
> 
> b) Beschreiben Sie die Funktionsweise

ANSWER

---

> a) Warum führt `copy_on_write` zur beschleunigten Ausführung eines child-Prozesses nach `fork()`
>
> b) Was geschieht, wenn einer der Prozesse eine Globalvariable modifiziert?
>
> c) Was geschieht bei einem Unterprogrammaufruf?

ANSWER

---

> **Copy-On-Write:**
>
> a) Was geschieht bei `fork()`?
>
> b) Was geschieht danach beim Ausführen von `exec()`?

ANSWER

---

> a) Warum wird bei Linux und Windows der Anwendungsadressraum von 4GB auf 3GB (Windows 2GB) verkleinert?
>
> b) Welche Vorteile hat diese Maßnahme bei einem Systemcall
>
> c) Welche Vorteile hat diese Maßnahme beim Datentransfer

ANSWER

---

> a) Was ist eine Race-Condition?
>
> b) Welche Fehler können auftreten?
>
> c) Wie kann man diese vermeiden?

ANSWER

---

> a) Was ist Feedback-Scheduling?
>
> b) Was will man damit erreichen?

ANSWER

---

> Fünf Aufträge warten auf ihren Start. Ihre erwarteten Laufzeiten sind 9, 5, 3 und 5 sec.
> In welcher Reihenfolge sollten sie laufen, damit die mittlere Antwortzeit minimiert wird?

ANSWER

---

> a) Warum werden Seiten ausgelagert?
>
> b) Was geschieht dabei?
>
> c) Welche Strategien gibt es?

---

> a) Was ist ein "Seitenfehler"?
>
> b) Wodurch wird er verursacht?
>
> c) Welche grundsätzlichen Reaktionen darauf gibt es?

---









## Virtualisierung

> Was ist ein Typ-1 Hypervisor und ein Typ-2 Hypervisor?

ANSWER

---

> Was ist die Voraussetzung eines Typ-1 Hypervisors?

ANSWER

---

> Was ist die Voraussetzung eines Typ-2 Hypervisors?

ANSWER

---

> Wie verhindert ein Typ-1 Hypervisor, dass ein Gastsystem direkt auf die Hardware zugreift?

ANSWER

---

> Wie verhindert ein Typ-2 Hypervisor, dass ein Gastsystem direkt auf die Hardware zugreift?

ANSWER

---

> **Bei modernen Systemen ist die Virtualisierung schon von Haus aus im Prozessor integriert.**
>
> a) Welchen zusätzlichen Hardwarebaustein braucht man, um Nested Page Tables zu unterstützten?
>
> b) Welche Eigenschaften msus ein Peripheriegerät vorweisen, um IO-Virtualisierung zu unterstützen?

ANSWER

---

> Was ist ein Container?

ANSWER

---

> Wie arbeitet ein System mit Containern?

ANSWER

---







## Systemaufrufe

> **Erklären Sie die Funktion und Wirkungsweise folgender System-Calls:**
>
> a) `fork()`
>
> b) `exec()`
>
> c) `wait()`
>
> d) `exit()`

---

> Beschreiben Sie den Ablauf eines Systemcalls am Beispiel des Aufrufs `write()` in eine Datei.

ANSWER

---

> Wozu dienen Interrupts ausgelöst durch Hardware?

ANSWER

---

> Wozu dienen Interrupts ausgelöst durch Software?

ANSWER

---








## Treiber

> Was ist ein Device-Switch-Table?

ANSWER

---

> Was bedeutet Minor- und Major-Number?

ANSWER

---

> Was sind 
> 
> a) Block-Devices
> b) Character Devices?

ANSWER

---

> Welche Aufgaben hat ein Gerätetreiber?

ANSWER

---

> Was versteht man unter "raw" und "cooked"?

ANSWER

---







## Dialogsysteme

> Beschreiben Sie die Funktionsweise eines Fenstersystems

ANSWER

---








## Unkategorisiert

> Welche Instruktionen eines Prozessors müssen privilegiert sein, um einen sicheren Betrieb eines Systems zu gewährleisten?

* Manipulation der Privilegstufen
* Manipulation der Adressierungsmechanismen
* Setzen der Interruptsperre
* Verwenden der I/O-Befehle

---

> a) Wie wird Shared Memory realisiert?
>
> b) Wozu wird es verwendet?