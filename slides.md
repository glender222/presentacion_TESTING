---
theme: default
background: https://images.unsplash.com/photo-1451187580459-43490279c0fa?q=80&w=1920&auto=format&fit=crop
class: text-center
highlighter: shiki
lineNumbers: false
aspectRatio: 16/9
transition: slide-left
fonts:
  sans: 'Inter'
  mono: 'Fira Code'
css: unocss
---

# Sistema de Gestión de Mensajería
### Identificación de Casos de Prueba — Entregable 1

<div class="mt-25 grid grid-cols-2 gap-10 text-left border-t border-white/20 pt-8">
  <div class="opacity-80">
    <span class="text-teal-400 font-bold uppercase text-xs">Integrantes</span>
    <p class="text-sm">Glender Vargas • Leroy Silva • Alejandro Apaza</p>
  </div>
  <div class="opacity-80">
    <span class="text-blue-400 font-bold uppercase text-xs">Curso</span>
    <p class="text-sm">Testing y Despliegue • 7mo Ciclo • Rogger Ubaldo</p>
  </div>
</div>

---
layout: two-cols
---

# Contexto y Solución

<div class="mr-4 mt-4 p-5 bg-red-900/10 border border-red-500/20 rounded-xl">
  <h2 class="text-red-400 font-bold mb-4">Problema</h2>
  <ul class="text-sm space-y-2 opacity-90">
    <li>• Desconexión Inventario vs WhatsApp</li>
    <li>• Respuestas lentas o incorrectas</li>
    <li>• Pérdida de ventas críticas</li>
    <li>• Alta carga operativa para administradores</li>
  </ul>
</div>

::right::

<div class="ml-4 mt-4 p-5 bg-teal-900/10 border border-teal-500/20 rounded-xl">
  <h2 class="text-teal-400 font-bold mb-4">Solución</h2>
  <ul class="text-sm space-y-2 opacity-90">
    <li>• Plataforma Web SaaS All-in-one</li>
    <li>• WhatsApp Multiagente centralizado</li>
    <li>• Chatbot con acceso a catálogo real</li>
    <li>• Centralización y mejora de conversión</li>
  </ul>
</div>

---
layout: two-cols
---

# Módulos del Sistema

::left::

<div class="mr-4 mt-6">
  <h2 class="text-blue-400 font-bold mb-4">Frontend</h2>
  <ul class="text-xs space-y-2 opacity-80">
    <li>• Login y acceso</li>
    <li>• Bandeja de conversaciones</li>
    <li>• Gestión de etiquetas</li>
    <li>• Gestión de bots y reglas</li>
    <li>• Gestión de empleados / estaciones</li>
    <li>• Historial / detalle del cliente</li>
  </ul>
</div>

::right::

<div class="ml-4 mt-6">
  <h2 class="text-teal-400 font-bold mb-4">Backend</h2>
  <ul class="text-xs space-y-1 opacity-80">
    <li>• Autenticación y sesión JWT</li>
    <li>• Gestión de estaciones de trabajo</li>
    <li>• Conexión y sesión de WhatsApp</li>
    <li>• Motor de chats y mensajería</li>
    <li>• Multimedia y gestión de archivos</li>
    <li>• Reglas y sesiones de bot</li>
  </ul>
</div>

---

# Alcance del Entregable

<div class="grid grid-cols-2 gap-8 mt-10 text-left">
  <div class="p-6 bg-teal-500/5 border border-teal-500/30 rounded-2xl">
    <h2 class="text-teal-400 font-bold mb-4 uppercase text-sm tracking-widest">Dentro del Alcance</h2>
    <ul class="text-sm space-y-2 opacity-90">
      <li>✔ Análisis funcional de frontend y backend</li>
      <li>✔ Identificación de casos por módulo</li>
      <li>✔ Matriz de casos detallada en Excel</li>
      <li>✔ Ambiente considerado: Certificación</li>
    </ul>
  </div>
  <div class="p-6 bg-red-500/5 border border-red-500/30 rounded-2xl">
    <h2 class="text-red-400 font-bold mb-4 uppercase text-sm tracking-widest">Fuera del Alcance</h2>
    <ul class="text-sm space-y-2 opacity-40">
      <li>✖ Ejecución de pruebas reales</li>
      <li>✖ Automatización de scripts</li>
      <li>✖ Evidencias de ejecución</li>
      <li>✖ Mediciones finales de rendimiento</li>
    </ul>
  </div>
</div>

---

# Criterio de Identificación

<div class="mb-8 bg-teal-900/30 p-3 rounded-lg border-l-4 border-teal-400 text-sm italic">
  "Consideramos flujos principales, alternativos, negativos, validaciones e interacción frontend-backend."
</div>

<div class="grid grid-cols-2 gap-10 text-left">
  <div>
    <h2 class="text-white font-bold mb-4 border-b border-white/10 pb-2">Frontend</h2>
    <ul class="text-xs space-y-1 opacity-70">
      <li>• Navegación por módulos</li>
      <li>• Validación de campos visuales</li>
      <li>• Permisos por rol de usuario</li>
      <li>• Interacción con formularios</li>
    </ul>
  </div>
  <div>
    <h2 class="text-white font-bold mb-4 border-b border-white/10 pb-2">Backend</h2>
    <ul class="text-xs space-y-1 opacity-70">
      <li>• Endpoints y lógica de negocio</li>
      <li>• Reglas de negocio y seguridad</li>
      <li>• Validaciones de datos y roles</li>
      <li>• Manejo de errores esperados</li>
    </ul>
  </div>
</div>

---

# Relación Académica y Metodológica

<div class="grid grid-cols-2 gap-8 mt-10 text-left">
  <div class="p-5 bg-white/5 rounded-xl border-l-4 border-yellow-500">
    <h3 class="font-bold text-yellow-500 mb-2">Modelo V</h3>
    <p class="text-xs opacity-80 leading-relaxed">Derivación de pruebas desde el diseño técnico y funcional para asegurar trazabilidad entre módulos e integración.</p>
  </div>
  <div class="p-5 bg-white/5 rounded-xl border-l-4 border-teal-500">
    <h3 class="font-bold text-teal-500 mb-2">Testing Ágil</h3>
    <p class="text-xs opacity-80 leading-relaxed">Trabajo iterativo por módulos, priorizando las funcionalidades críticas para el negocio en cada ciclo.</p>
  </div>
</div>

<div class="mt-12 flex justify-center gap-20 opacity-60">
  <div class="text-center">
    <p class="text-xl font-bold">ISO 25010</p>
    <p class="text-[10px] uppercase tracking-widest">Calidad</p>
  </div>
  <div class="text-center border-l border-white/20 pl-20">
    <p class="text-xl font-bold">ISO 29119</p>
    <p class="text-[10px] uppercase tracking-widest">Documentación</p>
  </div>
</div>

---

# Resumen de Casos de Prueba

<div class="grid grid-cols-3 gap-6 mt-6 items-center">
  <div class="col-span-2 overflow-hidden rounded-xl border border-white/10">
    <table class="w-full text-xs text-left">
      <thead class="bg-white/10 text-teal-400">
        <tr><th class="p-3">Módulo</th><th class="p-3 text-center">Backend</th><th class="p-3 text-center">Frontend</th></tr>
      </thead>
      <tbody class="opacity-80">
        <tr class="border-b border-white/5"><td class="p-2 pl-4">Autenticación / Seguridad</td><td class="text-center font-bold">14</td><td class="text-center">8</td></tr>
        <tr class="border-b border-white/5"><td class="p-2 pl-4">Chats y WhatsApp</td><td class="text-center font-bold">30</td><td class="text-center">10</td></tr>
        <tr class="border-b border-white/5"><td class="p-2 pl-4">Gestión de Bots</td><td class="text-center font-bold">38</td><td class="text-center">10</td></tr>
        <tr><td class="p-2 pl-4">Multimedia / Otros</td><td class="text-center font-bold">64</td><td class="text-center">22</td></tr>
      </tbody>
    </table>
  </div>

  <div class="bg-gradient-to-br from-teal-600/20 to-blue-600/20 p-8 rounded-3xl border border-white/20 text-center shadow-lg">
    <div class="text-6xl font-black text-teal-400 mb-2">196</div>
    <div class="text-[10px] uppercase font-bold tracking-widest opacity-60">Total Escenarios</div>
  </div>
</div>

---

# Ejemplos y Conclusiones

<div class="grid grid-cols-2 gap-4 mt-4 text-left">
  <div class="p-4 bg-blue-500/10 rounded-xl border-l-4 border-blue-500">
    <p class="text-xs text-blue-400 font-bold mb-1 uppercase">Frontend: Login vacío</p>
    <p class="text-[11px] opacity-80 italic">"No se envía el formulario; se muestran mensajes visuales de validación en la UI."</p>
  </div>
  <div class="p-4 bg-purple-500/10 rounded-xl border-l-4 border-purple-500">
    <p class="text-xs text-purple-400 font-bold mb-1 uppercase">Backend: Pass erróneo</p>
    <p class="text-[11px] opacity-80 italic">"Autenticación rechazada por API; mensaje de error controlado y sin token JWT."</p>
  </div>
</div>

<div class="mt-8 space-y-2 text-xs opacity-90">
  <p>✔ Análisis estructurado cubriendo lógica técnica y experiencia de usuario.</p>
  <p>✔ El análisis cubrió frontend y backend con mayor profundidad en lógica.</p>
  <p>✔ Excel queda como base coherente para la futura fase de ejecución.</p>
</div>


