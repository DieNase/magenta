# magenta
Das quelloffene Bildbearbeitungs- und Bildanalyse-Tool ImageJ erlaubt das Einbinden von eige-nen Funktionen in JAVA. Beispiel-Plugins sind vorhanden.
Es soll ein neues Plugin zur Farbraumtransformation RGB-> YUV programmiert werden, welches die Berechnungen V = R-G, U = B-G, Y = G+(U+V)/4 nicht zwangsläufig auf Basis von Werten an der aktuellen Position vornimmt, sondern auch Werte G aus der kausalen Nachbar-schaft zulässt. Welche Position genommen wird, hängt von Erfahrungen aus der Nachbarschaft ab. Ziel ist es, betragsmäßig möglichst kleine Werte für U und V zu erhalten. Als Güte-Kriterium dient die Summe der Entropien H(U)+ H(V)+ H(Y). Wichtig ist, dass die RGB-Werte eineindeu-tig wieder aus den YUV-Werten zurück gewonnen werden können: G = Y -(U+V)/4, B = U+G, R = V+G.
Das Plugin ist an verschiedenen Testbildern (Graustufen und Farbbilder) zu testen und die Kom-pressionsergebnisse sind zu dokumentieren.
Alle Untersuchungen sind schriftlich zu dokumentieren. Der Quellcode ist ausführlich zu kom-mentieren. Neben der schriftlichen Arbeit sind alle Quellen (Programmcode, Texte, Testbilder) und Tools abzugeben, damit eine Reproduktion der Ergebnisse möglich ist.

Beispiel Plugins:
https://github.com/imagej/tutorials
