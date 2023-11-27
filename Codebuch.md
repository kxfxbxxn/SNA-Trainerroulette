# Codebuch

## EDGE-Attribute

**from** 

ID des Herkunftsknotens  

Verein, der Trainer entlässt, oder Trainer, der zu Verein kommt

ID des Knoten Fußballverein bei type 1

ID des Knoten Fußballtrainer bei type 2
 
**to** 

ID des Zielknotens  

Verein, zu dem ein Trainer geht, oder Trainer, der einen Verein verlässt

ID des Knoten Fußballtrainer bei type 1

ID des Knoten Fußballverein bei type 2

**year**

Jahr des Trainerwechsels

**type** 

1 = Trainer verlässt Verein

2 = Trainer wechselt zu Verein

**pps**

Hier werden die Punkteausbeute pro Spiel sowie der Trainereffekt des Trainerwechsels angegeben. Bei type 1 wird die Punkteausbeute vor der Trainerentlassung berechnet, bei type 2 die Punkteausbeute nach dem Trainerwechsel. Der Bemessungszeitraum umfasst immer maximal fünf Spiele. Es kann aber auch zu einem Bemessungszeitraum von ein bis vier Spielen kommen, wenn der Trainer nur kürzer beim Verein war.

**effect**

Hier wurde der Trainereffekt **nur** für kommende Trainer berechnet, da abgehende Trainer keinen Einfluss mehr auf den Erfolg des ehemaligen Vereins haben. Der Trainereffekt wurde aus der Differenz zwischen den "pps" des Nachfolgetrainers und des abgehenden Trainers berechnet. Der Ergebnisbereich lag zwischen -3 (vorgehender Trainer = 3 pps, nachfolgender Trainer = 0 pps) und 3 (vorgehender Trainer = 0 pps, nachfolgender Trainer = 3 pps). Wir codierten den Effekt wie folgt:

**0,5** --\> -3 \< x \<= -2

**1** --\> -2 \< x \<= - 1

**2** --\> -1 \< x \< 0

**3** --\> x = 0

**4** --\> 0 \< x \< 1

**5** --\> 1 \<= x \< 2

**6** --\> 2 \<= x \< 3

x = Differenz der Punkte pro Spiel (pps).

## NODE-Attribute

**id** 

(eindeutige Codierung des Knoten) 

codiert von 1 bis 730, jede ID entspricht die Abkürzung eines Fußballtrainers oder eines Fußballvereins

**name** 

Vollständiger Name des Trainers / Vereins

**type** 

Art des Knoten

1 = Es handelt sich um einen Fußballtrainer

2 = Es handelt sich um einen Fußballverein

**league** 

Hier wird erfasst, in welcher erstklassigen Fußball-Liga sich der Fußballtrainer oder der Fußballverein befindet

1 = Bundesliga (Deutschland)

2 = Premier League (England)

3 = LaLiga (Spanien)

4 = Serie A (Italien)

5 = Ligue 1 (Frankreich)

6 = ligaübergreifender Trainer
