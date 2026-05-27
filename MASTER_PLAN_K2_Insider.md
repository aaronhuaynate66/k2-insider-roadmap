# MASTER_PLAN.md — K2 Insider Implementation

> **Objetivo raíz:** Activar el motor de captura y nurturing de leads B2B de K2 en Insider IN ONE antes del 30 de junio de 2026.
> Implementación completa de Email + Web Push + Onsite con perfilamiento conductual de decisores.

---

## 1. Estado General

| Campo | Valor |
|---|---|
| Proyecto | K2 Seguridad — Implementación Insider IN ONE |
| Cliente | K2 Seguridad y Resguardo SAC |
| Agencia | Aimo / Growthy y Marketing |
| Cuenta Insider | `k2aimo.inone.useinsider.com` (partnerId 10013744) |
| Épica Jira | GYM-1677 |
| Stack | Insider IN ONE · WordPress (k2.com.pe) · mineria.k2.com.pe |
| Estado global | 🟢 EN PROGRESO — bloque email 100% operativo |
| Deadline final | 2026-06-30 |
| Última actualización | 2026-05-27 |
| Maintainer | @aaronhuaynate66 |

---

## 2. Progreso General

​```
Tickets épica         : 9 (GYM-1838 → GYM-1846)
Tickets adicionales   : 2 (GYM-1969 coordinación AM, GYM-1981 PRO Elements)
Tickets cerrados      : 2  (GYM-1838, GYM-1839)
Tickets en curso      : 5  (GYM-1840, 1842, 1844, 1845, 1969)
Tickets por hacer     : 4  (GYM-1841, 1843, 1846, 1981)

Progreso técnico      : ████████░░░░░░░░░░░░  ~40%
Progreso de diseño    : █████████████████░░░  ~85%
Progreso global       : ████████████░░░░░░░░  ~60%
​```

---

## 3. Estado por Ticket

| Ticket | Nombre | Estado |
|---|---|---|
| GYM-1838 | Cuenta Insider creada y verificada | ✅ Cerrado |
| GYM-1839 | DNS — SPF/DKIM/DMARC | ✅ **Cerrado 27/05** — Mail Tester 10/10 |
| GYM-1840 | SDK + atributos + segmentos | 🟡 En curso · SDK k2.com.pe ✅, mineria pendiente |
| GYM-1841 | Plantillas email (16 emails, 4 series) | ⬜ Por hacer · Brief entregado |
| GYM-1842 | Diseño del journey B2B | 🟡 En curso · Esperando aprobación K2 |
| GYM-1843 | Construcción journey en Architect | ⬜ Por hacer · Prerequisites técnicos completos |
| GYM-1844 | Web Push opt-in + 2 automatizaciones | 🟡 En curso · Diseño listo |
| GYM-1845 | Onsite — popup, banner, exit intent | 🟡 En curso · Popup en Passive |
| GYM-1846 | QA completo + lanzamiento oficial | ⬜ Por hacer |
| GYM-1969 | Coordinación AM Aimo + Insider One | 🟡 En curso |
| GYM-1981 | Bug PRO Elements en wp-admin | ⬜ Por hacer |

---

## 4. Bloqueantes Actuales

| # | Bloqueante | Edad |
|---|---|---|
| B3 | Double Opt-in en Pending Review | 7 días |
| B5 | SDK no instalado en mineria.k2.com.pe | 2 días |
| B6 | Aprobación K2 del journey | 5 días |
| B7 | Aeylin redactando emails | — |

**Bloqueantes resueltos:**
- ✅ B1 — SDK sin enviar eventos (26/05: push de init)
- ✅ B2 — Volumen IP en -100.000 (27/05: Aaron tenía permisos)
- ✅ B4 — Industria como Retailers (no afecta operación)

---

## 5. Hitos Cerrados Recientes

| Fecha | Hito |
|---|---|
| 2026-05-25 | DNS publicado y verificado |
| 2026-05-25 | SDK instalado en k2.com.pe |
| 2026-05-26 | Master Plan publicado en GitHub |
| 2026-05-26 | Fix del SDK (push de init) |
| 2026-05-27 | Shared IP asignada |
| 2026-05-27 | Sender Address Setup confirmado |
| 2026-05-27 | Warm Up Plan generado |
| 2026-05-27 | **Mail Tester 10/10** |
| 2026-05-27 | **GYM-1839 cerrado como Finalizada** |

---

## 6. KPIs

| KPI | Target | Actual |
|---|---|---|
| Leads en 6 meses | 290 | 0 |
| Inbox placement | ≥95% | ✅ 100% al inbox principal |
| Mail Tester score | ≥9/10 | ✅ 10/10 |

---

*Última actualización: 2026-05-27 · Maintainer: @aaronhuaynate66*
