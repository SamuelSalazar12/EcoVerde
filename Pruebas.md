# Plan de Pruebas para EcoVerde

## Prueba 1: Búsqueda y Visualización de Plantas (Cobertura: RF-1, RF-2, RNF-1, RNF-3)
**Objetivo**: Verificar que los usuarios puedan encontrar y entender información de plantas

**Pasos**:
1. Ingresar término "Rosa" en búsqueda
2. Aplicar filtro "Exterior/Floral"
3. Seleccionar resultado "Rosa gallica"
4. Validar:
   - Escala de dificultad visible (RF-5)
   - Iconos de toxicidad para mascotas (RF-2)
   - Explicación simple de riego con imágenes (RNF-1)
5. Medir tiempo/pasos desde pantalla inicial (RNF-3)

**Criterio de Éxito**: Información completa obtenida en ≤4 interacciones

## Prueba 2: Gestión de Calendario (Cobertura: RF-3, RNF-4, RNF-5)
**Objetivo**: Probar creación y eliminación segura de recordatorios

**Pasos**:
1. Iniciar sesión con credenciales válidas (RF-6)
2. Acceder a "Mi Calendario"
3. Programar recordatorio de poda:
   - Fecha: 15/08
   - Hora: 09:00
   - Planta asociada: Lavanda
4. Intentar eliminar recordatorio:
   - Verificar diálogo de confirmación (RNF-5)
5. Validar posición consistente de botones (RNF-4)

**Criterio de Éxito**: Flujo completo sin errores y con salvaguardas

## Prueba 3: Guías Interactivas (Cobertura: RF-4, RNF-1, RNF-6)
**Objetivo**: Evaluar claridad de tutoriales

**Pasos**:
1. Buscar guía "Propagación por esquejes"
2. Verificar:
   - Diagramas animados legibles en zoom al 200% (RNF-6)
   - Lista de materiales con cantidades exactas
   - Instrucciones paso a paso con lenguaje simple (RNF-1)
3. Completar flujo hasta "Paso 3: Preparación del sustrato"

**Criterio de Éxito**: Usuario prueba comprende proceso sin ayuda externa

## Prueba 4: Sistema de Dificultad (Cobertura: RF-5, RNF-2)
**Objetivo**: Validar filtrado por nivel de experiencia

**Pasos**:
1. Usar filtro "Principiante" en explorador
2. Verificar contraste texto/fondo en resultados (RNF-2)
3. Seleccionar "Suculenta Echeveria"
4. Confirmar:
   - Badge de dificultad visible
   - Recomendaciones acordes al nivel
5. Cambiar filtro a "Avanzado" y repetir validación

**Criterio de Éxito**: Coherencia entre nivel y contenido sugerido

## Prueba 5: Conocimiento Local (Cobertura: RF-7, RNF-3)
**Objetivo**: Probar integración de saberes regionales

**Pasos**:
1. Activar GPS (simular ubicación en Puebla, MX)
2. Buscar "Cempasúchil"
3. Validar sección "Consejos Locales":
   - Técnicas de cultivo tradicionales
   - Fechas de siembra alineadas con festividades
4. Medir accesibilidad (≤3 taps desde pantalla principal) (RNF-3)

**Criterio de Éxito**: Datos georreferenciados precisos y accesibles

## Matriz de Cobertura

| Requisito | Prueba 1 | Prueba 2 | Prueba 3 | Prueba 4 | Prueba 5 | Cobertura |
|-----------|----------|----------|----------|----------|----------|-----------|
| RF-1      | ✓        |          |          |          |          | 100%      |
| RF-2      | ✓        |          | ✓        |          |          | 100%      |
| RF-3      |          | ✓        |          |          |          | 100%      |
| RF-4      |          |          | ✓        |          |          | 100%      |
| RF-5      | ✓        |          |          | ✓        |          | 100%      |
| RF-6      |          | ✓        |          |          |          | 100%      |
| RF-7      |          |          |          |          | ✓        | 100%      |
| RNF-1     | ✓        |          | ✓        |          |          | 100%      |
| RNF-2     |          |          |          | ✓        |          | 100%      |
| RNF-3     | ✓        |          |          |          | ✓        | 100%      |
| RNF-4     |          | ✓        |          |          |          | 100%      |
| RNF-5     |          | ✓        |          |          |          | 100%      |
| RNF-6     |          |          | ✓        |          |          | 100%      |