# MASTER_PLAN.md — K2 Insider Implementation

> Objetivo raíz: Activar el motor de captura y nurturing de leads B2B de K2 en Insider IN ONE antes del 30 de junio de 2026.

> Implementación completa de Email + Web Push + Onsite con perfilamiento conductual de decisores.

---

## 1. Estado General

| Campo | Valor |

|---|---|

| Proyecto | K2 Seguridad — Implementación Insider IN ONE |

| Cliente | K2 Seguridad y Resguardo SAC |

| Agencia | Aimo / Growthy y Marketing |

| Cuenta Insider | k2aimo.inone.useinsider.com (partnerId 10013744) |

| Épica Jira | GYM-1677 |

| Stack | Insider IN ONE · WordPress (k2.com.pe) · mineria.k2.com.pe (vanilla HTML/JS) |

| Estado global | 🟢 EN PROGRESO — bloque email 100% operativo, pendientes 3 fixes en mineria |

| Deadline final | 2026-06-30 |

| Última actualización | 2026-05-29 |

| Maintainer | @aaronhuaynate66 |

---

## 2. Progreso General

```
Tickets épica         : 9 (GYM-1838 → GYM-1846)
Tickets adicionales   : 3 (GYM-1969 coordinación, GYM-1981 PRO Elements, GYM-2029 diseño visual popup)
Tickets cerrados      : 2  (GYM-1838, GYM-1839)
Tickets en curso      : 5  (GYM-1840, 1842, 1844, 1845, 1969)
Tickets en espera     : 1  (GYM-1841)
Tickets por hacer     : 4  (GYM-1843, 1846, 1981, 2029)
Progreso técnico      : ██████████░░░░░░░░░░  ~50%
Progreso de diseño    : █████████████████░░░  ~85%
Progreso global       : █████████████░░░░░░░  ~65%
```

---

## 3. Estado por Ticket

| Ticket | Nombre | Estado |

|---|---|---|

| GYM-1838 | Cuenta Insider creada y verificada | ✅ Cerrado |

| GYM-1839 | DNS — SPF/DKIM/DMARC | ✅ Cerrado 27/05 — Mail Tester 10/10 |

| GYM-1840 | SDK + atributos + segmentos | 🟡 En curso · k2.com.pe ✅, mineria pendiente 3 fixes |

| GYM-1841 | Plantillas email (4 series · 16 emails) | 🟠 EN ESPERA · 4 shells creados, brief entregado a Aeylin |

| GYM-1842 | Diseño del journey B2B | 🟡 En curso · Esperando aprobación K2 |

| GYM-1843 | Construcción journey en Architect | ⬜ Por hacer · Prerequisites técnicos completos |

| GYM-1844 | Web Push opt-in + 2 automatizaciones | 🟡 En curso · Service Worker desbloqueado |

| GYM-1845 | Onsite — popup, banner, exit intent | 🟡 En curso · Popup en Passive |

| GYM-1846 | QA completo + lanzamiento oficial | ⬜ Por hacer |

| GYM-1969 | Coordinación AM Aimo + Insider One | 🟡 En curso · Volumen ✅, Double Opt-in pivoteado |

| GYM-1981 | Bug PRO Elements en wp-admin | ⬜ Por hacer · Fuera de épica |

| GYM-2029 | Diseño visual del Popup en editor Insider (manual) | ⬜ Por hacer · ~30-40 min |

---

## 4. Shells de Plantillas Creados en Insider (para Aeylin)

| # | Nombre | URL del editor |

|---|---|---|

| 1 | K2 — Plantilla 1 — Bienvenida (Email 1 del Journey) | https://k2aimo.inone.useinsider.com/email/templates/112842 |

| 2 | K2 — Plantilla 2 — Educativo / Valor (Email 2 del Journey) | https://k2aimo.inone.useinsider.com/email/templates/112843 |

| 3 | K2 — Plantilla 3 — Caso de Éxito / Social Proof (Email 3 del Journey) | https://k2aimo.inone.useinsider.com/email/templates/112845 |

| 4 | K2 — Plantilla 4 — CTA Comercial / Conversión (Email 4 del Journey) | https://k2aimo.inone.useinsider.com/email/templates/112846 |

---

## 5. Bloqueantes Actuales

| # | Bloqueante | Edad | Acción |

|---|---|---|---|

| B5 | SDK en mineria.k2.com.pe sin 3 fixes (init + sintaxis v2.x + checkbox consent) | 3 días | Colega notificado 28/05 y 29/05, esperando deploy |

| B6 | Aprobación K2 del journey | 6 días | Pendiente compartir entregables con K2 (deadline 02/06) |

| B7 | Aeylin entregando Serie A | — | Deadline sábado 31/05, shells listos |

Bloqueantes resueltos:

- ✅ B1 — SDK k2.com.pe sin enviar eventos (26/05: push de init)

- ✅ B2 — Volumen IP en -100.000 (27/05: Aaron tenía permisos, Shared IP asignada)

- ✅ B3 — Double Opt-in pending 8 días → pivoteado a Single Opt-in (revierte ADR-008)

- ✅ B4 — Industria como Retailers (no afecta operación)

---

## 6. Hitos Cerrados Recientes

| Fecha | Hito |

|---|---|

| 2026-05-25 | DNS publicado y verificado |

| 2026-05-25 | SDK instalado en k2.com.pe (vía WPCode) |

| 2026-05-26 | Master Plan publicado en GitHub |

| 2026-05-26 | Fix del SDK aplicado (push de init) — eventos llegando |

| 2026-05-27 | Shared IP asignada (1.000/mes, daily 100) |

| 2026-05-27 | Sender Address Setup confirmado (K2 Seguridad · marketing@k2.com.pe) |

| 2026-05-27 | Warm Up Plan generado y confirmado |

| 2026-05-27 | Mail Tester 10/10 · Email Setup completo |

| 2026-05-27 | GYM-1839 cerrado oficialmente |

| 2026-05-28 | Limpieza de campañas duplicadas en Web Templates |

| 2026-05-28 | 4 shells de plantillas creados en Insider para Aeylin |

| 2026-05-28 | Decisión: Double Opt-in → Single Opt-in (revierte ADR-008) |

| 2026-05-28 | Verificación SDK mineria.k2.com.pe (detectados 2 issues iniciales) |

| 2026-05-28 | GYM-1841 transicionado a EN ESPERA · GYM-2029 creado |

| 2026-05-28 | 7 worklogs registrados (~33h acumuladas) · 8 links de dependencia |

| 2026-05-29 | Verificación mineria: colega no aplicó los 3 fixes — segundo mensaje enviado con código exacto |

---

## 7. Decisiones Arquitectónicas (ADRs)

| ADR | Decisión | Estado |

|---|---|---|

| ADR-001 | DNS gestionados directamente en GoDaddy por Aaron (sin esperar IT) | ✅ Aplicado |

| ADR-002 | SDK k2.com.pe vía plugin WPCode (no edición de tema) | ✅ Aplicado |

| ADR-003 | Scoring del formulario en frontend (JavaScript) | ✅ Diseñado |

| ADR-004 | Subdominio técnico em6900.k2.com.pe para envío Insider | ✅ Aplicado |

| ADR-005 | NO publicar SPF de SendGrid en k2.com.pe | ✅ Aplicado |

| ADR-006 | Soft Ask para opt-in de Web Push (no nativo directo) | ✅ Diseñado |

| ADR-007 | Unbranded shortened links para tracking de email | ✅ Aplicado |

| ADR-008 | Double Opt-in en lugar de Single | ❌ Revertido 28/05 → Single Opt-in |

| ADR-008b | Single Opt-in con checkbox de consentimiento explícito en form | 🟡 Pendiente deploy (mineria) |

| ADR-009 | Journey con 4 ramas (no 3 como en spec original) | ✅ Diseñado |

| ADR-010 | Routing del journey por perfil_decisor | ✅ Diseñado |

| ADR-011 | Push de {type: 'init'} requerido en WPCode | ✅ Aplicado (k2.com.pe) · 🟡 Pendiente (mineria) |

| ADR-012 | Volumen email k2aimo: 1.000/mes, daily 100, Shared IP | ✅ Aplicado |

| ADR-013 | Warm-up de 1 día (no curva multi-día) | ✅ Aplicado |

| ADR-014 | Subscriber Base skipped temporal (espera validación Tag 48-72h) | ✅ Pivote temporal |

| ADR-015 | Unsubscribe Groups y Pages en "No" para v1 | ✅ Aplicado |

---

## 8. KPIs del Proyecto

| KPI | Target | Actual |

|---|---|---|

| Leads en 6 meses | 290 | 0 (esperando lanzamiento) |

| Open rate del journey | ≥35% | — |

| Click rate del journey | ≥5% | — |

| Inbox placement | ≥95% | ✅ 100% al inbox principal |

| Mail Tester score | ≥9/10 | ✅ 10/10 |

| Tasa opt-in efectiva Web Push | ≥12% | — |

| User Profiles acumulados | — | 219 (k2.com.pe activo) |

---

## 9. Tareas Pendientes Documentadas

1. Mineria — Fix #1: push de init en <head> (sin esto, los otros 2 fixes son irrelevantes)

2. Mineria — Fix #2: reemplazar handler v1.x del form por sintaxis v2.x (objetos)

3. Mineria — Fix #3: agregar checkbox de consentimiento al form (Single Opt-in)

4. Global Unsubscribe → reactivar con Yes cuando entre el primer lead real (compliance CAN-SPAM/GDPR)

5. Web SDK como Subscriber Base method → cuando Insider valide Tag Integration (48-72h del crawler)

6. Postmaster Tool Setup → opcional pero recomendable para reputación en Gmail

7. Cambiar Email Consent Type en Insider de Double Opt-in a Single Opt-in (espera confirmación de checkbox en form)

8. Diseño visual del Popup → ~30-40 min manuales en editor de Insider (GYM-2029)

9. Logo K2 oficial → subir al popup y plantillas

10. Plantillas custom con branding K2 → Aeylin debe diseñar (no usar default Insider One)

11. GYM-1981 PRO Elements → fuera de épica pero conviene resolver

12. WhatsApp a Insider Support → forzar validación manual del Tag para k2.com.pe (cookie banner bloquea crawler)

---

## 10. Siguiente Acción Inmediata

```
🎯 PROYECTO EN BUENA POSICIÓN
   Email Setup 100% operativo. 3 fixes pendientes en mineria.
   Aeylin entrega Serie A sábado 31/05. K2 aprobación lunes 02/06.
```

Esperando terceros:

- [ ] Colega de mineria aplica 3 fixes (segundo mensaje enviado 29/05)

- [ ] Aeylin entrega Serie A (deadline sábado 31/05)

- [ ] K2 aprueba journey (deadline lunes 02/06)

- [ ] Insider Support valida Tag manualmente (WhatsApp por mandar)

Acciones sin terceros:

- [ ] WhatsApp a Insider Support (Aaron, ~5 min)

- [ ] Diseño visual del Popup en Insider (Aaron manual, ~30-40 min)

Cuando mineria aplique los 3 fixes:

- [ ] Verificar end-to-end (hit + lead_captured con email_optin)

- [ ] Cambiar Email Consent Type en Insider de Double Opt-in a Single Opt-in

- [ ] Cerrar GYM-1840 al 100%

---

Última actualización: 2026-05-29 · Maintainer: @aaronhuaynate66
