# Manual de uso — Calculadora de Costeo JCM

Esta herramienta te dice si un proyecto es rentable y a qué precio cotizarlo. No necesitas saber de ingeniería ni de contabilidad — solo ingresar los números que te den.

---

## Cómo abrir la calculadora

1. Busca el archivo **calculadora_jcm.html** en tu teléfono o computadora
2. Hazle doble clic (o tócalo en el teléfono)
3. Se abre sola en el navegador (Chrome, Safari, Edge — cualquiera sirve)
4. No necesita internet ni cuenta en ningún lado

---

## Parte 1 — Qué ingresar

### Costos del proyecto

**Materiales**
El total que pagaste (o que te cotizaron) por los materiales, con ITBIS incluido. Es el número que aparece en la factura del suplidor. Si no hay materiales, déjalo en cero.

**Mano de obra / subcontrata**
Lo que cobra la persona que va a hacer el trabajo físico. Puede ser:
- Un subcontratista que contratan
- Joseph mismo — en ese caso se coloca igual, es lo que cobra por su tiempo

**Viáticos / combustible**
Gasolina, peajes, comida en campo. Si no hay, déjalo en cero.

---

### ¿Quién ejecuta el trabajo?

**Yo mismo**
Joseph hace el trabajo. La mano de obra va 100% a su bolsillo — no es un gasto de la empresa.

**Subcontratista formal**
La persona tiene RNC (está registrada en impuestos). Sin cargos adicionales.

**Subcontratista informal**
La persona no tiene RNC. Aparecen retenciones de impuestos automáticamente. Hay que elegir:
- **Técnico · 2%** — electricistas, instaladores
- **Profesional · 10%** — ingenieros con honorarios

---

### Complejidad / Colchón de imprevistos

Porcentaje que cubre lo que no se ve venir en la obra.

- **Baja · 5%** — proyecto simple, ya hecho antes
- **Media · 10%** — proyecto normal (usar esto si hay duda)
- **Alta · 15%** — proyecto complejo o situación nueva

---

### Parámetros de precio

| Campo | Valor normal | Para qué sirve |
|---|---|---|
| Margen objetivo % | 22 | Cuánto se quiere ganar |
| Descuento máx. % | 10 | Máximo que puedes bajar si el cliente negocia |
| Margen mínimo % | 15 | Si la ganancia cae aquí, el proyecto no conviene |
| Colchón % | 10 | Mismo que seleccionaste arriba |

No cambies estos valores a menos que Joseph te indique otra cifra.

**Redondear techo hacia arriba**
El precio final se redondea al múltiplo elegido. Lo normal es **1,000** — así el precio queda limpio (ej. 207,000 en vez de 206,842).

---

### Cliente exento (Zona Franca)

Actívalo si el cliente es empresa de Zona Franca (como GTS). Significa que no le cobras ITBIS encima del precio. El precio base no cambia.

---

### Vendedor externo

Si alguien trajo el proyecto y tiene comisión, activa este toggle y elige el rol:

- **Referidor · 4%** — solo pasó el contacto
- **Gestor · 6%** — coordinó reuniones y dio seguimiento
- **Socio cierre · 8%** — negoció y cerró

La comisión va dentro del precio — la paga el cliente, no sale de la ganancia de JCM.

---

## Parte 2 — Cómo leer los resultados

### La luz de arriba (semáforo del proyecto)

- 🟢 **VIABLE** — el proyecto da bien, incluso si el cliente negocia
- 🟡 **VIABLE — AJUSTADO** — da, pero con poco margen. No dar más descuento
- 🔴 **NO VIABLE** — con ese descuento el proyecto no es rentable. Hay que revisar costos o subir el precio

---

### Precio a cotizar

El número grande en verde-azul es el precio que le presentas al cliente.

Debajo aparece:
- **Piso real** — el mínimo que puedes aceptar. Debajo de ese número el proyecto pierde sentido
- **Si das −X%** — qué precio quedaría si el cliente negocia ese descuento (verde = OK, rojo = no conviene)

El cuadro pequeño muestra tu bolsillo y el margen si das ese descuento. Verde = puedes ceder. Rojo = no.

Si el cliente no es exento, aparece también el total con ITBIS — ese es el número real que paga el cliente.

---

### Costo total real

Todo lo que sale de tu bolsillo antes de ganar algo:
- Materiales con ITBIS
- Subcontrata (y su ITBIS si es informal)
- Viáticos
- Colchón de imprevistos

---

### Análisis de ganancia

- **Ganancia bruta** — precio menos costos
- **− ISR 27%** — impuesto fijo por ley
- **Ganancia neta** — lo que queda limpio
- **Tu bolsillo (50%)** — mitad para Joseph personalmente
- **+ Tu mano de obra** — aparece solo cuando Joseph ejecuta; va 100% a él
- **Tu bolsillo TOTAL** — lo que realmente entra al bolsillo de Joseph
- **Fondo empresa (50%)** — la otra mitad queda en JCM
- **Margen neto real** — porcentaje de ganancia real sobre el precio

---

### Panel DGII (fondo amarillo, solo con subcontratista informal)

No afecta el precio — es solo para los reportes de impuestos:

- Cuánto le pagas en mano al subcontratista
- Cuánto retienes de ITBIS → remitir al IT-1 antes del **día 20** del mes siguiente
- Cuánto retienes de ISR → remitir al IR-17 antes del **día 10** del mes siguiente

---

## Botones

**Cargar caso PISANO** — carga un proyecto real validado para ver cómo funciona. Útil para practicar o explicarle a alguien.

**Limpiar** — borra los campos de costos para empezar un proyecto nuevo.

---

## Regla de oro

La calculadora te dice si el proyecto **da o no da** y a qué precio cotizar. Si el cliente pide rebaja, mira el cuadro de descuento — verde puedes ceder, rojo no. Cualquier duda, llama a Joseph.
