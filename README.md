# 🎛️ PulmoFlow — Interaktywny Symulator Respiratora 

> **Strona demonstracyjna live:** [borshiik.github.io/Respirator-simulator](https://borshiik.github.io/PulmoFlow/)

Interaktywna strona prezentacyjna (landing page) oraz demonstracja internetowa projektu **PulmoFlow** — zaawansowanego systemu szkoleniowego przeznaczonego dla lekarzy, pielęgniarek i ratowników medycznych do nauki rozpoznawania i eliminacji asynchronii pacjent–respirator.

---

## 🌐 O projekcie

**PulmoFlow** to innowacyjny symulator medyczny, który wypełnia lukę między drogimi symulatorami klinicznymi a podstawowymi modelami programowymi. Ten katalog zawiera kod interaktywnej witryny promocyjnej i demonstracyjnej, która wizualizuje respirator w trójwymiarowym środowisku WebGL bezpośrednio w przeglądarce.

---

## ✨ Funkcje prezentacji 3D

- **Interaktywny Model 3D:** Możliwość obracania, przybliżania i interakcji z modelem 3D urządzenia PulmoFlow stworzonym przy użyciu React Three Fiber.
- **Wykresy WebGL w czasie rzeczywistym:** Dynamiczne, płynne wykresy krzywych oddechowych (ciśnienie, przepływ, objętość) renderowane bezpośrednio na ekranie 3D z prędkością 60 FPS za pomocą zoptymalizowanych buforów linii WebGL.
- **Wielowątkowa Fizyka (Web Worker):** Pętla fizycznej symulacji płuc (solver RK4 - Runge-Kutta 4. rzędu) została przeniesiona do osobnego wątku w tle (`physics.worker.js`), dzięki czemu ruch kamery i animacje strony pozostają idealnie płynne.
- **Nowoczesny Design:** Ciemny interfejs (Dark Mode) z płynnymi gradientami CSS, sprzętowo przyspieszanymi cząsteczkami w tle (`<Sparkles>`) oraz realistycznymi cieniami kontaktowymi.
- **Pełna responsywność:** Układy dopasowane i przetestowane pod kątem urządzeń mobilnych, tabletów i komputerów stacjonarnych.

---

## 🛠️ Użyte technologie

- **Silnik 3D:** Three.js / [@react-three/fiber](https://github.com/pmndrs/react-three-fiber) / [@react-three/drei](https://github.com/pmndrs/drei)
- **Fizyka:** Wielowątkowy solver RK4 oparty o Web Workers
- **Warstwa wizualna:** HTML5 + Vanilla CSS3 (Flexbox/Grid) + Vite
- **Hosting:** GitHub Pages

---

## 🚀 Uruchomienie lokalne

Aby uruchomić stronę demonstracyjną lokalnie na swoim komputerze:

### 1. Zainstaluj zależności
```bash
npm install
