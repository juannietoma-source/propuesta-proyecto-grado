# Validación y Verificación del Proyecto  
### Sistema de Facturación Empresarial  
 

---

## 1. Introducción

Este documento presenta las actividades de **validación y verificación (V&V)** aplicadas al proyecto **Sistema de Facturación Empresarial**.  
El propósito es garantizar que el sistema cumpla con las necesidades del usuario y con los requisitos técnicos establecidos.

- **Validación:** Determina si el sistema satisface las necesidades del usuario final.  
- **Verificación:** Evalúa si el sistema se construye correctamente conforme a las especificaciones y estándares de diseño.

---

## 2. Objetivos de la V&V

- Asegurar la coherencia, completitud y corrección de los requisitos.  
- Confirmar que cada componente cumple con su diseño y funcionalidad esperada.  
- Detectar y corregir errores antes del desarrollo final.  
- Establecer trazabilidad entre requisitos, casos de uso y pruebas.

---

## 3. Alcance de la Validación y Verificación

| Etapa del Proyecto | Tipo de Actividad | Descripción |
|--------------------|------------------|--------------|
| Análisis | Validación | Revisión de requisitos e historias de usuario con el cliente. |
| Diseño | Verificación | Análisis de consistencia de diagramas UML y estructura de base de datos. |
| Implementación | Verificación | Pruebas unitarias y de integración del código. |
| Pruebas | Validación | Pruebas de aceptación de usuario y simulación de uso real. |
| Documentación | Verificación | Revisión de manuales técnico y de usuario. |

---

## 4. Casos de Uso Identificados

| ID | Nombre del Caso de Uso | Actor Principal | Descripción | Tipo (Validar/Verificar) |
|----|------------------------|-----------------|--------------|---------------------------|
| CU01 | Registrar cliente | Administrador | Permite registrar y administrar clientes. | Validar |
| CU02 | Registrar producto | Administrador | Crea productos con precio, IVA y stock. | Verificar |
| CU03 | Emitir factura | Vendedor | Genera facturas con cálculo automático de IVA y descuentos. | Validar |
| CU04 | Exportar factura a PDF | Vendedor | Exporta la factura a formato PDF con logo e información completa. | Verificar |
| CU05 | Generar reportes | Administrador | Obtiene reportes de ventas por rango de fechas en PDF/Excel. | Validar |
| CU06 | Control de inventario | Administrador | Actualiza el stock al facturar y muestra productos con bajo inventario. | Verificar |
| CU07 | Sistema de autenticación y roles | Todos | Controla el acceso según rol (admin, vendedor, contador). | Verificar |
| CU08 | Panel de métricas | Administrador | Muestra gráficas de ventas diarias y productos más vendidos. | Validar |

---

## 5. Tabla de Trazabilidad

| Requisito | Caso de Uso Relacionado | Prueba Asociada | Estado Esperado |
|------------|------------------------|-----------------|-----------------|
| RQ01 - Registrar clientes | CU01 | Prueba de inserción en BD | Cliente registrado correctamente |
| RQ02 - Gestión de productos | CU02 | Prueba de validación de campos y stock | Producto creado y listado |
| RQ03 - Facturación | CU03 | Prueba de cálculo de IVA y total | Factura generada correctamente |
| RQ04 - Exportar factura | CU04 | Prueba de generación de PDF | Archivo PDF descargado |
| RQ05 - Reportes | CU05 | Prueba de rango de fechas | Reporte mostrado correctamente |
| RQ06 - Control de inventario | CU06 | Prueba de stock descontado | Stock actualizado |
| RQ07 - Autenticación | CU07 | Prueba de inicio y cierre de sesión | Acceso permitido/denegado |
| RQ08 - Panel de métricas | CU08 | Prueba de visualización gráfica | Datos representados correctamente |

---

## 6. Actividades de Validación

1. Revisión de requisitos con el cliente.  
2. Validación de flujos mediante prototipos o mockups.  
3. Evaluación de consistencia de historias de usuario.  
4. Simulación de escenarios de facturación, inventario y reportes.  

---

## 7. Actividades de Verificación

1. Revisión técnica de diseño y base de datos.  
2. Validación de formato y coherencia de reportes.  
3. Pruebas unitarias en módulos de facturación, login e inventario.  
4. Revisión de seguridad en contraseñas y roles.  
5. Validación del funcionamiento de exportación PDF/Excel.  

---

## 8. Resultados Esperados

- Cada historia de usuario cumple con sus criterios de validación.  
- Los módulos principales funcionan sin errores críticos.  
- Los reportes y métricas reflejan datos reales del sistema.  
- El código cumple buenas prácticas de programación.  
- Documentación técnica y manual de usuario verificados.  

---

## 9. Conclusión

La aplicación de validación y verificación permitirá reducir errores antes de la implementación final del sistema y asegurar que el producto cumpla con las expectativas del cliente y los objetivos definidos en la propuesta original.  

---

## 10. Archivos Relacionados

- `/diagrams/usecase_diagram.png` — Diagrama de Casos de Uso  
- `/docs/validation_verification.md` — Documento actual  
- `/tests/unit/` — Carpeta para pruebas unitarias  
- `/tests/integration/` — Carpeta para pruebas de integración  

---

**Autor:** Juan Felipe Nieto Manjarres  


  

