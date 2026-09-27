# Centinela — Plataforma operativa de escalado

Repositorio que documenta la estructura operativa, las metodologías ágiles
y el backlog de escalado de **Centinela**, una solución de validación de
identidad y detección de fraude sintético (deepfakes) en tiempo real para
transacciones financieras.

Este repositorio es el radiador de información del Trabajo Práctico Tema 2
(Diseño de la Estructura Operativa, Procesos y Marcos de Trabajo — ASI 2026)
y complementa al Informe Técnico Consolidado entregado en PDF/Word.

## Qué vas a encontrar acá

- **Project (tablero Kanban):** ver la pestaña *Projects* del repositorio.
  Columnas: Backlog → Refined (DoR) → In Progress → Code Review / PR →
  QA / Testing → Staging → Done (DoD).
- **Issues:** las 8 Historias de Usuario del backlog de escalado (Épica 1:
  Autenticación escalable / Épica 2: Escalado del motor de detección),
  cada una con criterio INVEST y aceptación en formato BDD/Gherkin.
- **Labels:** identifican Squad, Épica y clase de servicio (`expedite`,
  `standard`, `fixed-date`, `intangible`).
- **[POLICIES.md](./POLICIES.md):** Definition of Ready y Definition of Done
  vigentes para todo el equipo.

## Equipos (Team Topologies)

| Squad | Tipo | Responsabilidad |
|---|---|---|
| Core IA | Stream-aligned | Motor de detección de medios sintéticos |
| Identidad & Autenticación | Stream-aligned | RBAC, SSO/SAML |
| Onboarding & Integraciones | Stream-aligned | API modular, documentación |
| Plataforma / MLOps / DevOps | Platform | Infraestructura, CI/CD, observabilidad |
| SecOps & Compliance | Enabling | Auditoría GDPR, seguridad |
| Confiabilidad y Soporte (SRE) | Ops | Guardia 24/7, incidentes |

## Autores
Bettiol Giuliana · Sanchez Juan — Administración de Sistemas de Información, 2026
