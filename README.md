# Abgabe Deep Learning

## Abgabe bis 05.01.2024

Florian Paul

Link zu Binder:
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/FlorianDHBWFN/Abgabe_DeepLearning.git/HEAD?urlpath=Abgabe.ipynb)


## Zusammenfassung und Diskussion:

Die Verwendung der Convolutional-Schichten führt auf jeden Fall zu einer Verbesserung
des Modells. Bei der Verwendung des gesamten Trainingsdaten des MNIST-Datensatzes
wird eine Accuracy von 99,61 % erreicht. Auch wenn das Modell nur noch mit 5000 Trainingsbildern
(und damit einem zwölftel der vorher verwendeten Daten) wird das vorher
gesteckte Ziel von mindestens 98 % Validation Accuracy erreicht. Damit ist das neue
Modell in der Validation Accuracy besser als das die Vorlage. Dies ist aber nur möglich
durch die Verwendung von Datenaugmentierung. Dadurch wird insgesamt eine Accuracy
von 98,15 % erreicht. Eine speicherplatzeffiziente Lösung wird durch ein nicht zu großes
Model mit ca. 225034 Parametern erreicht. Dies ist möglich durch die Verwendung der
Pooling-Layer. Aus diesem Zweck ist auch nur eine Dense-Schicht verwendet worden.
Des Weiteren werden zu diesem Zweck die augmentierten Bilder nur während der einzelnen
Epochen des Trainings gespeichert und anschließend wieder verworfen. Durch diese
Implementierung ist jedoch die Anzahl der augmentierten Bilder begrenzt.
Es könnte mit einer größeren Anzahl an augmentierten Bildern eine höhere Accuracy
erreichen. Aufgrund der Speichereffizienz wurde darauf jedoch verzichtet.
Zusammenfassend kann gesagt werden, dass das Modell eine Validation Accuracy von
98,15 % hat, welche damit höher ist als in der Vorlage. Das Modell weist 225034 Parameter
auf und des wurden für das Training 5000 Label verwendet.