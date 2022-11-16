# 09foeppingerRandom

# Random

#Warum könnte man den Zufall beim Programmieren brauchen?

Zum Beispiel für einen "Casinosimulator" in welchem die Wahrscheinlichkein wie oft zum beispiel eine sechs gewürfelt wird varrieren soll.
Um Item droprates zu bestimmen...


#Was ist der Unterschied zwischen Random aus System bzw. aus UnityEngine?
Gib jeweils ein Beispiel.

Nun, es gibt nur 2 große Unterschiede: UnityEngine.Random ist eine statische Klasse, also werden wir nur einen Generator von Zufallszahlen pro Spiel haben. Mit System.Random müssen Sie mindestens einen instanziieren, oder Sie können mehrere Zufallsgeneratoren mit verschiedenen Seeds gleichzeitig instanziieren.


#Warum ist es sinnvoll den seed zu setzen bei Random?

Es ist deterministisch und die Sequenz, die es generiert, wird durch den Seed-Wert bestimmt, an den Sie übergeben random.seed. Normalerweise rufen Sie einfach auf random.seed () und es verwendet die aktuelle Zeit als Startwert, was bedeutet, dass Sie bei jeder Ausführung des Skripts eine andere Folge von Werten erhalten. 

#Was macht Random.Range?

maxExcusive ist exklusiv, so dass beispielsweise Random.Range (0, 10) einen Wert zwischen 0 und 9 zurückgibt, jeweils mit ungefähr gleicher Wahrscheinlichkeit. Wenn minInclusive und maxExclusive gleich sind, wird die "exklusive Regel" ignoriert und minInclusive zurückgegeben. Wenn minInclusive größer als maxExclusive ist, werden die Nummern automatisch vertauscht.
