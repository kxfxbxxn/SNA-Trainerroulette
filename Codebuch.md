# Codebuch

## EDGE-Attribute

Wert,Kommentar
edgelist,
from,"ID des Herkunftsknotens (Verein, der Trainer entlässt, oder Trainer, der zu Verein kommt)"
to,"ID des Zielknotens (Verein, zu dem ein Trainer geht, oder Trainer, der einen Verein verlässt)"
type,"1 = Trainer geht von einem Verein weg, 2 = Trainer kommt zum Verein"
pps,Die durchschnittliche Anzahl der Punkte in den letzten / ersten fünf Spielen vor Abgang / Neu-Transfer 
effect,"Der Trainereffekt codiert in Zahlen - von 0,5 bis 6"
nodelist,

## NODE-Attribute

**id**

(eindeutige Codierung des Knoten)   
Kürzel des Trainers / Vereins (Kombination aus Vor- und Nachname / Vereinsname)

**name** 

Vollständiger Name des Trainers / Vereins

**type**
1 = Trainer
2 = Verein

**league**
1 = Bundesliga
2 = Premier League
3 = LaLiga
4 = Serie A
5 = Ligue 1
6 = ligaübergreifender Trainer
