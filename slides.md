---
theme: default
background: https://images.unsplash.com/photo-1451187580459-43490279c0fa?q=80&w=1920&auto=format&fit=crop
class: text-center
highlighter: shiki
lineNumbers: true
aspectRatio: 16/9
transition: slide-left
fonts:
  sans: 'Inter'
  serif: 'Georgia'
  mono: 'Fira Code'
css: unocss
---

# Sistema de Gestión de Mensajería y más

Identificación de Casos de Prueba — Entregable 1

<div class="pt-12 text-sm text-left grid grid-cols-2 gap-4">
  <div>
    <strong>Integrantes:</strong><br/>
    Glender Vargas<br/>
    Leroy Silva<br/>
    Alejandro Apaza
  </div>
  <div>
    <strong>Curso:</strong> Testing y Despliegue<br/>
    <strong>Docente:</strong> Rogger Ubaldo<br/>
    <strong>Ciclo:</strong> 7mo ciclo
  </div>
</div>

<!--
Abrir indicando que se presentará el primer entregable enfocado
en la identificación de casos de prueba de la solución.
-->

---
layout: two-cols
---

# Contexto del proyecto y solución propuesta

Startup SaaS en etapa MVP orientada a PYMEs de LATAM con foco inicial en Perú.

::left::

## Problema

<v-clicks>

- **Desconexión** entre inventario, ventas online y conversaciones de WhatsApp
- **Efectos:**
  - Respuestas lentas o incorrectas
  - Pérdida de ventas
  - Alta carga operativa
- **Usuarios afectados:**
  - Dueños / administradores
  - Agentes de ventas y atención
  - Cliente final

</v-clicks>

::right::

## Solución

<v-clicks>

- **Plataforma web SaaS all-in-one**
- **Integra:** 
  - Inventario
  - WhatsApp multiagente
  - Chatbot con acceso a catálogo
- **Beneficios:**
  - Centralización
  - Reducción de errores
  - Mejor tiempo de respuesta
  - Aumento de conversión

</v-clicks>

<!--
Enfatizar que la solución nace de un problema real de operación y no de
una idea abstracta. Esta parte cubre la definición de la solución que pesa en la rúbrica.
-->

---
layout: two-cols
---

# Módulos del sistema: frontend y backend

::left::

## Frontend

<v-clicks>

- Login y acceso
- Bandeja de conversaciones
- Gestión de etiquetas
- Gestión de bots y reglas
- Gestión de empleados / estaciones
- Historial / detalle del cliente

</v-clicks>

::right::

## Backend

<v-clicks>

- Autenticación y sesión de usuario
- Gestión de empleados / estaciones de trabajo
- Conexión y sesión de WhatsApp
- Chats y mensajería
- Etiquetas y acceso a chats
- Multimedia y archivos
- Bots
- Reglas de bot
- Sesiones de bot

</v-clicks>

<!--
Aclarar que el backend tiene mayor detalle técnico porque concentra reglas de negocio,
roles, validaciones e integraciones. Esto responde a la sección de "descripción de módulos"
de la rúbrica.
-->

---
layout: default
---

# Alcance del entregable

<div class="grid grid-cols-2 gap-8 mt-10">
  <div class="bg-teal-500/10 p-6 rounded-lg border border-teal-500/30">
    <h2 class="text-teal-400 font-bold mb-4">Dentro del Alcance</h2>
    <ul class="list-disc pl-5">
      <li v-click="1">Análisis de frontend y backend</li>
      <li v-click="2">Identificación de casos de prueba por módulo</li>
      <li v-click="3">Documentación completa en Excel</li>
      <li v-click="4">Ambiente considerado: <strong>Certificación</strong></li>
    </ul>
  </div>
  <div class="bg-red-500/10 p-6 rounded-lg border border-red-500/30">
    <h2 class="text-red-400 font-bold mb-4">Fuera del Alcance</h2>
    <ul class="list-disc pl-5 text-gray-400">
      <li v-click="5">Ejecución de pruebas</li>
      <li v-click="6">Automatización</li>
      <li v-click="7">Evidencias</li>
      <li v-click="8">Mediciones finales de rendimiento</li>
    </ul>
  </div>
</div>

<!--
Decir claramente que esta fase corresponde a identificación de casos, no a ejecución,
tal como se indicó en clase.
-->

---
layout: two-cols
---

# Criterio usado para identificar los casos de prueba

<div class="mb-4 bg-teal-900/40 px-4 py-2 rounded-lg border-l-4 border-teal-400">
  <span class="text-sm font-bold text-teal-300 uppercase tracking-widest">Flujos considerados:</span> 
  principales · alternativos · negativos · validaciones · interacción frontend-backend
</div>

::left::

## Criterios Frontend

<v-clicks>

- Navegación por módulos
- Validación de campos
- Mensajes visuales
- Permisos por rol
- Interacción con formularios

</v-clicks>

::right::

## Criterios Backend

<v-clicks>

- Endpoints
- Reglas de negocio
- Validaciones
- Roles y permisos
- Errores esperados
- Integraciones

</v-clicks>

<div class="col-span-2 mt-8" v-click="12">
  <blockquote class="border-l-4 border-teal-500 bg-teal-500/10 p-4 rounded-r-lg">
    <span class="text-xl italic font-serif">"No solo identificamos casos funcionales, sino también escenarios negativos, validaciones e interacción entre frontend y backend."</span>
  </blockquote>
</div>

<!--
Esto está alineado con lo visto en clase: un caso de prueba parte de entradas,
condiciones y resultados esperados, y debe cubrir flujo básico y alternativos.
-->

---
layout: two-cols
---

# Relación con lo visto en clase

::left::

## Modelo V

<v-clicks>

- Diseño del sistema dividido en módulos
- Derivación de pruebas desde el diseño técnico y funcional
- Relación entre: 
  - Módulos
  - Integración
  - Sistema
  - Aceptación futura

</v-clicks>

::right::

## Testing Ágil

<v-clicks>

- Trabajo por módulos
- Identificación iterativa
- Prioridad a funcionalidades críticas
- Posibilidad de ampliar casos en ciclos siguientes

</v-clicks>

<div class="col-span-2 mt-8 bg-gray-800 p-4 rounded-lg flex items-center gap-4 border border-gray-700" v-click>
  <div class="i-carbon-certificate text-4xl text-yellow-500"></div>
  <div>
    <div class="font-bold text-sm text-yellow-400">SOPORTE METODOLÓGICO</div>
    <div class="text-sm text-gray-300">
      <strong>ISO/IEC 25010:</strong> Atributos de calidad <br/>
      <strong>ISO/IEC/IEEE 29119:</strong> Documentación de pruebas
    </div>
  </div>
</div>

<!--
El modelo V relaciona diseño y pruebas por niveles, el testing ágil justifica trabajar
por módulos y priorizar lo crítico. La mención a ISO es solo respaldo metodológico.
-->

---
layout: default
---

# Resumen de casos de prueba identificados

<div class="grid grid-cols-2 gap-8 text-sm mt-4">

<div>

<h3 class="text-teal-400 mb-2 border-b border-teal-400/30 pb-1">TABLA BACKEND</h3>

| Módulo                          | Casos | Prioridad |
| :---                            | :---: | :---:     |
| Autenticación y sesión          |  14   |  Alta     |
| Gestión de empleados            |  14   |  Media    |
| Conexión y sesión de WhatsApp   |  12   |  Alta     |
| Chats y mensajería              |  18   |  Alta     |
| Etiquetas y acceso a chats      |  22   |  Alta     |
| Multimedia y archivos           |  14   |  Media    |
| Bots                            |  16   |  Alta     |
| Reglas de bot                   |  22   |  Alta     |
| Sesiones de bot                 |  14   |  Media    |
| **TOTAL BACKEND**               | **146**|          |

</div>

<div>

<h3 class="text-blue-400 mb-2 border-b border-blue-400/30 pb-1">TABLA FRONTEND</h3>

| Módulo                          | Casos | Prioridad |
| :---                            | :---: | :---:     |
| Login y acceso                  |   8   |  Alta     |
| Bandeja de conversaciones       |  10   |  Alta     |
| Gestión de etiquetas            |   8   |  Media    |
| Gestión de bots y reglas        |  10   |  Alta     |
| Gestión de empleados/estaciones |   8   |  Media    |
| Historial / detalle del cliente |   6   |  Media    |
| **TOTAL FRONTEND**              |  **50**|          |

<div class="mt-8 text-center bg-gradient-to-r from-teal-600/20 to-blue-600/20 py-6 rounded-lg border border-teal-500/30 shadow-lg">
  <div class="text-4xl font-black text-transparent bg-clip-text bg-gradient-to-r from-teal-400 to-blue-400">196</div>
  <div class="text-sm uppercase tracking-wide text-gray-300 mt-2 font-bold">Casos Identificados en Total</div>
</div>

</div>

</div>

<!--
Esta es la diapositiva clave para la rúbrica del PPT. Debe verse muy ordenada.
Los módulos con más riesgo identificados fueron WhatsApp, chats, etiquetas y reglas de bot.
-->

---
layout: default
---

# Ejemplos representativos y conclusiones

<div class="grid grid-cols-2 gap-6 my-6">

<div class="bg-gray-800/80 p-5 rounded-xl border-l-4 border-blue-500 shadow-md">
  <div class="text-blue-400 font-bold mb-3 flex items-center gap-2">
    <div class="i-carbon-laptop text-xl"></div> Ejemplo Frontend
  </div>
  <div class="font-bold text-white mb-2">Login con campos vacíos</div>
  <div class="text-sm text-gray-300">
    <div class="text-teal-400 font-semibold mb-1">Resultado esperado:</div>
    No se envía el formulario, se muestran mensajes de validación visuales y el usuario permanece en la vista de acceso.
  </div>
</div>

<div class="bg-gray-800/80 p-5 rounded-xl border-l-4 border-purple-500 shadow-md">
  <div class="text-purple-400 font-bold mb-3 flex items-center gap-2">
    <div class="i-carbon-server text-xl"></div> Ejemplo Backend
  </div>
  <div class="font-bold text-white mb-2">Login con contraseña incorrecta</div>
  <div class="text-sm text-gray-300">
    <div class="text-teal-400 font-semibold mb-1">Resultado esperado:</div>
    Autenticación rechazada, mensaje de error correspondiente por API y no se entregan tokens de acceso.
  </div>
</div>

</div>

<h2 class="mt-8 mb-4">Conclusiones</h2>

<ul class="text-[0.95rem] space-y-2 text-gray-200">
  <li v-click="1"><span class="text-teal-400 mr-2">✔</span> Se identificaron de manera estructurada los casos de prueba más relevantes.</li>
  <li v-click="2"><span class="text-teal-400 mr-2">✔</span> El análisis cubrió frontend y backend, con mayor profundidad técnica en backend.</li>
  <li v-click="3"><span class="text-teal-400 mr-2">✔</span> Se consideraron flujos básicos, alternativos, validaciones y roles.</li>
  <li v-click="4"><span class="text-teal-400 mr-2">✔</span> El Excel queda como base para una futura fase de ejecución y validación.</li>
  <li v-click="5"><span class="text-teal-400 mr-2">✔</span> La PPT y el Excel mantienen coherencia entre módulos, escenarios y cantidad de casos.</li>
</ul>

<!--
Cerrar diciendo que el valor de este entregable no está en "probar por probar",
sino en haber construido una base ordenada, coherente y trazable para las
siguientes fases. En clase se remarcó que los casos de prueba reflejan
requerimientos, cubren flujo básico y alternativo, y deben ser claros,
precisos y consistentes.
-->
