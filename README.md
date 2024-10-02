# PLZ-Entfernungen in Deutschland

Dieses Repository enthält Entfernungsdaten zwischen deutschen Postleitzahlen (PLZ), wobei ausschließlich Distanzen von weniger als 50 km berücksichtigt wurden. Die Daten wurden erstellt, um Berechnungen zwischen verschiedenen Orten in Deutschland zu erleichtern. Sie können in Projekten verwendet werden, die geografische Analysen oder die Suche nach Orten basierend auf PLZ und einem bestimmten Radius erfordern.

Die zugrunde liegenden Daten stammen von der Plattform [Opendatasoft](https://public.opendatasoft.com/explore/dataset/georef-germany-postleitzahl/export/), die öffentlich zugängliche Informationen bereitstellt.

## Datenformat

Die Entfernungsdaten sind in zwei Formaten verfügbar:

1. **CSV-Datei**: Die Daten sind in der Datei `plz_distances.csv` im folgenden Format gespeichert:

   | PLZ_1  | PLZ_2  | Entfernung (km) |
   |--------|--------|-----------------|
   | 01067  | 01067  | 0               |
   | 01067  | 01069  | 3               |
   | 01067  | 01097  | 2               |
   | 01067  | 01099  | 8               |
   | 01067  | 01108  | 11              |
   | ...    | ...    | ...             |

   Jede Zeile enthält zwei PLZ und die jeweilige Entfernung zwischen diesen beiden Postleitzahlen in Kilometern.

3. **JSON-Datei**: Die Daten sind auch in der Datei `graph.json` im folgenden Format gespeichert:

   ```json
   {
     "01067": {
       "01067": 0,
       "01069": 3,
       "01097": 2,
       "01099": 8,
       "01108": 11,
       "01109": 7,
       "01127": 4,
       "01129": 4,
       "01139": 3,
       "01156": 7,
       "01157": 4,
       "01159": 2,
       "01169": 4,
       "01187": 5
     }
   }
