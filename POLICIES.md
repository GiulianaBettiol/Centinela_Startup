# Políticas de calidad — Centinela

Estas políticas son de cumplimiento obligatorio para todos los Squads antes
de mover una tarjeta entre columnas del tablero. Se referencian desde el
[README](./README.md) y desde la descripción del Project.

## Definition of Ready (DoR)

Una Historia de Usuario **no puede entrar a "In Progress"** sin cumplir:

- [ ] Cumple el checklist **INVEST** (Independiente, Negociable, Valiosa,
      Estimable, Small, Testeable).
- [ ] Los criterios de aceptación están redactados en formato **BDD/Gherkin**
      (Dado / Cuando / Entonces).
- [ ] Los mockups o el diseño de API relevantes están aprobados por el
      Tech Lead o UX.
- [ ] Las dependencias técnicas con otros squads están identificadas y
      resueltas, o al menos acordadas con el squad correspondiente.
- [ ] La historia tiene asignada su Épica, su Squad y su clase de servicio
      (labels correspondientes cargadas).

## Definition of Done (DoD)

Una Historia de Usuario **no puede moverse a "Done"** sin cumplir:

- [ ] Pruebas unitarias con cobertura **≥ 80%**.
- [ ] Análisis estático de código (**SAST**) sin vulnerabilidades críticas.
- [ ] Revisión de código (**Pull Request**) aprobada por al menos un par.
- [ ] Documentación de API actualizada (OpenAPI) si corresponde.
- [ ] Desplegado exitosamente en ambiente de **staging** con smoke tests
      aprobados.

## Clases de servicio

| Clase | Cuándo se usa | Regla en el tablero |
|---|---|---|
| **Expedite** | Incidentes críticos o caídas de producción | Ingresa sin respetar el WIP limit; atención en enjambre (swarming) de todo el squad disponible |
| **Standard** | Historias planificadas del flujo normal | Sigue el orden FIFO habitual del backlog |
| **Fixed Date** | Compromiso contractual o regulatorio con fecha límite | Se prioriza a medida que se acerca la fecha límite |
| **Intangible** | Refactorización y deuda técnica | Reserva fija del 20% de la capacidad del squad por sprint |

## Límites de trabajo en progreso (WIP)

| Columna | Límite |
|---|---|
| In Progress | 6 tarjetas |
| Code Review / PR | 4 tarjetas |
| QA / Testing | 3 tarjetas |
