# dynamicStemma

This software generates a dynamic stemma (slideshow)

#Citation
If you use any of this, please cite:
@INPROCEEDINGS{Hoenen:2016,
    booktitle={DHd 2016 Konferenzabstracts},
    author={Hoenen, Armin},
    year={2016},
    title={Das erste dynamische Stemma, Pionier des digitalen Zeitalters?},
    url = {http://www.dhd2016.de/abstracts/posters-060.html}
  }

#Walkthrough
1. Sie entpacken das zip-File irgendwo
2. Sie öffnen ein Windows commandprompt oder ein Terminal (Eingabeaufforderung)
3. Sie navigieren in den entzippten Ordner (meist mit "cd " + Pfadnamen)
4. Sie rufen im Ordner den Befehl "java -jar dynamicStemma.jar" auf
    - sie werden nacheinander um die Eingabe einer Bildunterschrift,
      des Stemma im Newickformat
      und der Kantensequenz gebeten*
5. Nach Ende der Berechnung befindet sich imselben Ordner ein File "run.sh" und ein File "run.bat"
    - sollten Sie Linux nutzen, rufen Sie einfach "sh run.sh" auf
    - bei Windows müssten Sie auf run.bat doppelklicken; hier kann es sein, dass die die 3 .bat Dateien
      sowie alle .tex Dateien erst in das Verzeichnis ihrer LaTeX installation kopieren müssen, oder aber Sie
      müssen alle .tex Dateien mit ihrem LaTeX Editor öffnen und dort von Hand kompilieren (zuerst die testframes
      und erst am Ende die dynStem.tex
    - was sie für Mac tun müssen, entzieht sich meiner Kenntnis, allerdings glaube ich es wird wie in Linux ablaufen

Jetzt sollten sie die pdf Datei "dynStem.pdf" generiert haben, auf der 2ten Seite desselbigen befindet sich ihr dynamisches Stemma.


Sollte es Versionierungskonflikte oder andere Probleme geben, können Sie mir auch gerne ihre
Stemmata als Newick und ihre Edgesequenzen im genannten Format zuschicken und ich schicke Ihnen das Resultat.

*das Kantensequenzformat ist noch einmal angepasst worden und mehrere Kanten in einem Sequenzschritt werden nun durch "&" getrennt. Z.B.:   Alpha-m1&Alpha-Beta;Beta-m3 ... 
