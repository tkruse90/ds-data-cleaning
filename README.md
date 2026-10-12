# Datenbereinigung

Eine praxisnahe Einführung in die Bereinigung eines echten, unordentlichen Datensatzes mit pandas. Anhand einer rohen Wetterdatei aus Seattle korrigierst du Spaltennamen, entfernst Duplikate, korrigierst Datentypen und Einheiten, vereinheitlichst kategoriale Bezeichnungen und gehst mit fehlenden Werten um. Die Datenbereinigung ist ein Teil der explorativen Datenanalyse (EDA), daher bildet dieses Notebook eine Grundlage für dein erstes Projekt.

## Lernziele

Am Ende dieses Repositorys solltest du in der Lage sein:

- einen Rohdatensatz zu untersuchen und typische Probleme der Datenqualität zu erkennen,
- Spaltennamen zu vereinheitlichen und doppelte Zeilen zu entfernen,
- Datentypen zu korrigieren und Werte zu transformieren: Datumsangaben, Einheiten und kategoriale Bezeichnungen,
- mit fehlenden Daten umzugehen, indem du Zeilen entfernst oder Werte imputierst (Konstante, Mittelwert/Median/Modus, Interpolation),
- fehlende Werte mit missingno zu visualisieren, um nach Mustern zu suchen.

## Lernpfad

| Datei / Ordner | Beschreibung |
|---|---|
| [**01 - Datenbereinigung**](01_data_cleaning.ipynb) | Bereinige einen rohen Wetterdatensatz aus Seattle von Anfang bis Ende: untersuchen, Spaltennamen korrigieren, Duplikate entfernen, Datentypen und Einheiten korrigieren, kategoriale Werte zuordnen und fehlende Daten imputieren. |

### Weitere Ordner und Dateien

| Datei / Ordner | Beschreibung |
|---|---|
| [**Data**](data/) | Der im Notebook verwendete Rohdatensatz `seattle-weather_raw.csv`. |
| [**Solutions**](solutions/) | Musterlösungen für die Übungen. |
| [**pyproject.toml**](pyproject.toml) | Projektkonfiguration und Abhängigkeiten. |
| [**uv.lock**](uv.lock) | Lock-Datei für die Abhängigkeiten. |

## Einrichtung

> [!NOTE]
> In den folgenden Schritten ist Text in spitzen Klammern wie `<repo-name>` ein **Platzhalter**. Ersetze ihn einschließlich der Klammern `< >` durch deinen eigenen Wert. Aus `cd <repo-name>` wird zum Beispiel `cd ds-data-cleaning`.

### 1. Repository aus dem Template erstellen

Klicke auf GitHub auf **Use this template**.

Beim Erstellen des Repositorys:

- Lege dich selbst als **Owner** fest
- Wähle einen Namen für das Repository
- Deaktiviere **Include all branches**
- Klicke auf **Create repository**

> [!IMPORTANT]
> Wenn ihr zu zweit oder in Gruppen arbeitet, sollte nur **eine Person** diesen Schritt ausführen.

---

### 2. Mitwirkende hinzufügen (nur bei Paar- oder Gruppenarbeit)

Wenn du mit anderen zusammenarbeitest:

1. Öffne das Repository auf GitHub
2. Gehe zu **Settings → Collaborators**
3. Füge deine Teammitglieder als Collaborators hinzu
4. Teile den Link zum Repository mit deinem Team

Deine Teammitglieder sollten die Einladung annehmen, bevor es weitergeht.

---

### 3. Repository klonen

Kopiere die SSH-URL über den Button **Code** auf GitHub und führe dann aus:

```bash
git clone <kopierte-ssh-url>
```

Die kopierte SSH-URL sieht etwa so aus: `git@github.com:<dein-username>/<repo-name>.git`.

---

### 4. In den Projektordner wechseln und Abhängigkeiten installieren

Damit werden alle Abhängigkeiten installiert und eine virtuelle Umgebung in `.venv/` erstellt.

```bash
cd <repo-name>
uv sync
```

---

### 5. Notebook öffnen

> [!NOTE]
> Öffne VS Code unbedingt aus dem Hauptverzeichnis des Projekts, damit die von `uv sync` erstellte Umgebung automatisch erkannt wird.

Starte VS Code im Hauptverzeichnis des Projekts:

```bash
code .
```

Öffne dann `01_data_cleaning.ipynb` und wähle die von `uv sync` erstellte Python-Umgebung als Kernel aus.

## Quellen und weiterführende Literatur

Die verlinkten Ressourcen sind auf Englisch.

- [**Pandas: Working with missing data**](https://pandas.pydata.org/docs/user_guide/missing_data.html): Offizieller Leitfaden zum Erkennen, Entfernen und Auffüllen fehlender Werte.
- [**Pandas: Getting started tutorials**](https://pandas.pydata.org/docs/getting_started/intro_tutorials/index.html): Kurze, praxisnahe Einführungen in den grundlegenden pandas-Workflow.
- [**Pythonic data cleaning with pandas and NumPy**](https://realpython.com/python-data-cleaning-numpy-pandas/): Ein ausführliches Tutorial, das dieselben Bereinigungsschritte auf andere echte Datensätze anwendet.
- [**Kaggle: Data Cleaning course**](https://www.kaggle.com/learn/data-cleaning): Ein kurzer, kostenloser Kurs mit Übungen zu fehlenden Werten, Skalierung und inkonsistenten Texteinträgen.
