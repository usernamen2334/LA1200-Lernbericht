# LA1200-Lernbericht
Lernbericht für Gruppenprojekt LA1200

# Lern-Bericht
Gruppe Elephant: Angelov, Atputharasa, Marku, Tanner, von Rogall

## Einleitung

In unserem Projekt geht es um eine Anmeldung für verschiedene Workshops. Dies haben wir in Visual Studio in C# implementiert. Der Benutzer kann zwischen verschiedenen Workshops auswählen. Man soll als Benutzer seine drei Prioritäten eingeben können und anhand dieser in den passenden Workshop eingeteilt werden. Wenn alle Teilnehmer eingegeben wurden, wird eine Liste ausgegeben. Dort sieht man welche Workshops stattfinden und wo die Teilnehmer eingeteilt sind. 

In unserem Code haben wir mehrmals Switch-Case angewendet, sind nun sicher beim Verwenden und wissen auch wann wir es am besten verwenden. Dazu möchten wir in diesem Lernbericht noch näher kommen.

## Beschreibung


Switch-Case hat im Prinzip dieselbe Funktion wie if und else. Es sorgt dafür dass, wenn ein Benutzer etwas bestimmtes eingibt (Fall), die darauf folgende Aktion auf den Fall abgestimmt ist. Bei if und else ist das ganze aber sehr unübersichtlich und in die Länge gezogen, denn man müsste für jeden einzelnen Fall einen neuen if/else Befehl erstellen. Hingegen bei Switch-Case kann man alle möglichen Fälle beieinander erstellen und es herrscht Ordnung. Mit dem Befehl "switch" beginnt man und kann danach beliebig viele "case" erstellen, also Fälle. Am Ende kommt noch ein "default" dazu, der sorgt dafür, dass bei einer Fehleingabe das Programm nicht einfach abstürzt. Anstelle dessen gibt es eine Fehlermeldung aus und bittet den Benutzer nochmals eine Eingabe zu tätigen, welche korrekt ist. Switch-Case haben wir oft verwendet, da es uns sehr geholfen hat die Übersicht zu behalten. Wir konnten somit die vielen Bedingungen unseres Programmes gut unterbringen.


 Console.Write(namen[durchlauf / 3] + " > Kurs " + (i + 1) + " auswählen: ");
                        int eingabe = Convert.ToInt32(Console.ReadLine());
                        if (eingabe >= 1 && eingabe <= 5)
                        { 
                            switch(i)
                            {
                                case 0:
                                    e1 = eingabe;
                                    break;
                                case 1:
                                    e2 = eingabe;
                                    if (e2 == e1) { throw new Exception(); }
                                    break;
                                case 2:
                                    e3 = eingabe;
                                    if (e3 == e1 || e3 == e2) { throw new Exception(); }
                                    break;
                                default:
                                    break;
                            }
                         }   
                         
In diesem Code Fetzten geht es darum, dass der Benutzer drei Prioritäten setzt. Als erstes haben wir "Switch(i)",  also wissen wir jetzt, dass eine Switch-Case kommt und wie sie bennent ist. Danach kommen unsere drei "Case", unsere Fälle. Das geschriebene (e2==e1) sorgt dafür, dass die gesetzte zweite Priorität nicht die gleiche wie die erste ist, das wird deutlich gemacht mit "throw new expection". Am Schluss dann noch der "default", für die Fehlermeldung. Oben wird noch mit einer if/else Bedingung sichergestellt, dass die Eingabe zwischen 1-5 ist, da es nur 5 Kurse gibt.

* Ein deutliches, aussagekräftiges Bild oder eine kommentierte Bildschirm-Aufnahme

## Verifikation

Switch-Case zu verstehen ist nicht allzu schwierig. Mit der Texterklärung von oben, welche das Prinzip vom Ganzen erklärt sollte es verständlich gemacht werden. Der Code-Fetzten zeigt das Ganze dann in der Praxis und man kann sein Wissen nun auch noch auf dem eingefügten Bild anwenden und sollte den Aufbau verstehen. Wenn man die Grafik sieht kann man gut erkennen was der Text beschreibt und versteht es somit auch besser, weil man es sieht. 

# Reflektion zum Arbeitsprozess

Unser Team harmoniert sehr gut zusammen und wir pflegen eine gute Kommunikation, was uns vieles erleichterte. Die Arbeitspakete waren gut aufgeteilt und wir hatten insgesamt einen guten Überblick. 

Wir waren am Anfang ein wenig überfordert was das gemeinsame arbeiten am Programm anging, wie wir den Code gemeinsam bearbeiten könnten. Nachdem wir uns aber einen Ratschlag geholt haben, konnten wir ohne Probleme weiterarbeiten.

Wir zögerten beim nachfragen für Hilfe und versuchten es alleine zu lösen, das nächste mal sollten wir direkt Hilfe holen ohne zögern, um Zeit zu sparen.
