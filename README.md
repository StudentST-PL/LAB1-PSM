# LAB1-PSM - Jetpack Compose

Aplikacja zrealizowana w ramach laboratoriów z Programowania Systemów Mobilnych (PSM).
Jest to prosta interaktywna wizytówka, która pozwala na ukrywanie i pokazywanie danych użytkownika po kliknięciu przycisku.

**Technologie:**
* Język: Kotlin
* Interfejs użytkownika: Jetpack Compose

## Porównanie podejść: Jetpack Compose vs Views (Java + XML)

| Zagadnienie | Jetpack Compose (Kotlin)                                                                          | Views (Java + XML) |
| :--- |:--------------------------------------------------------------------------------------------------| :--- |
| **Liczba plików do edycji** | 2 pliki (`MainActivity.kt`, `strings.xml`). Kod UI i logika siedzą w jednym miejscu.              | 4 pliki (`build.gradle.kts`, układ XML, `strings.xml`, `MainActivity.java`). |
| **Czas kompilacji** | Pierwsza kompilacja bywa dłuższa, ale `@Preview` pozwala na szybką iterację bez pełnego restartu. | Kompilacja szybka, ale testowanie logiki widoków wymaga pełnego przeładowania aplikacji. |
| **Czytelność kodu** | Bardzo wysoka. Kod zwięzły, brak boilerplate'u, ukrywanie elementów naturalnym warunkiem `if`.    | Przeciętna. Rozbicie na XML i Javę zaciemnia główną logikę biznesową. |

**Wniosek końcowy:** Podejście Jetpack Compose okazało się znacznie czytelniejsze, ponieważ eliminuje narzut związany z synchronizacją plików XML z kodem logiki, pozwalając definiować interfejs w sposób deklaratywny.