# ¿Qué tan cuántica es la nube?
**Diagnóstico experimental de entrelazamiento, decoherencia y deriva en hardware de IBM Quantum**

Proyecto desarrollado para el *Paper del Mes* — IEEE Computer Society PUCP Student Branch Chapter.

## Objetivo
Utilizar las desigualdades de Bell (CHSH) y Mermin como sondas de caracterización (*benchmarking*) para cuantificar la calidad del entrelazamiento, el tiempo efectivo de coherencia cuántica, la escalabilidad multipartita y la deriva temporal en procesadores superconductores de IBM Quantum.

## Protocolo Experimental
- **E0:** Validación en simulador ideal y con modelo de ruido (`qiskit-aer`).
- **E1:** Mapeo espacial del parámetro $S$ en pares de qubits adyacentes.
- **E2:** Barrido angular $\theta \in [0, 2\pi]$ para estimar la visibilidad $V$.
- **E3:** Decaimiento temporal $S(t)$ frente a tiempos de espera (*delay*) y comparación con $T_2$.
- **E4:** Violación de desigualdades de Mermin en estados GHZ de $N$ qubits.
- **E5:** Pruebas de reproducibilidad interdiaria (*drift*) y verificación de no-señalización.
