# Sistema de Gestión de Eventos Educativos

Sistema web para la gestión de eventos, ubicaciones y contactos en instituciones educativas, desarrollado con React, TypeScript y Supabase.

## Características

- Gestión completa de eventos (conferencias, talleres, seminarios)
- Administración de ubicaciones con coordenadas geográficas
- Gestión de contactos con información detallada
- Interfaz intuitiva siguiendo principios de HCI
- Diseño responsivo para todos los dispositivos
- Dashboard con estadísticas en tiempo real

## Tecnologías

- **Frontend**: React 18 + TypeScript
- **Estilos**: Tailwind CSS
- **Base de Datos**: Supabase (PostgreSQL)
- **Iconos**: Lucide React
- **Build Tool**: Vite

## Instalación

```bash
# Clonar el repositorio
git clone [URL_DEL_REPOSITORIO]

# Instalar dependencias
npm install

# Configurar variables de entorno
# Crear archivo .env con:
# VITE_SUPABASE_URL=tu_url_de_supabase
# VITE_SUPABASE_ANON_KEY=tu_clave_de_supabase

# Ejecutar en desarrollo
npm run dev

# Compilar para producción
npm run build
```

## Estructura del Proyecto

```
src/
├── App.tsx              # Componente principal
├── main.tsx            # Punto de entrada
├── lib/
│   └── supabase.ts     # Cliente de base de datos
└── components/
    ├── Layout.tsx      # Layout principal
    ├── Dashboard.tsx   # Panel de control
    ├── Events.tsx      # Módulo de eventos
    ├── Locations.tsx   # Módulo de ubicaciones
    └── Contacts.tsx    # Módulo de contactos
```

## Funcionalidades

### Eventos
- Crear, editar, eliminar y listar eventos
- Clasificación por tipo (Conferencia, Taller, Seminario)
- Asociación con ubicaciones
- Gestión de invitados y recordatorios
- Configuración de zona horaria y repetición

### Ubicaciones
- CRUD completo de ubicaciones
- Dirección y coordenadas geográficas
- Integración con Google Maps

### Contactos
- Gestión de participantes y conferencistas
- Información de contacto completa
- Soporte para fotografías

## Base de Datos

El sistema utiliza tres tablas principales:

- `events`: Información de eventos
- `locations`: Lugares físicos
- `contacts`: Participantes y conferencistas

Todas las tablas incluyen Row Level Security (RLS) para acceso público controlado.

## Principios de HCI Aplicados

- **Visibilidad**: Elementos interactivos claramente identificables
- **Feedback**: Respuesta visual inmediata a acciones del usuario
- **Consistencia**: Diseño uniforme en toda la aplicación
- **Prevención de errores**: Validación de formularios y confirmaciones
- **Affordance**: Elementos que sugieren su función

## Despliegue

La aplicación está desplegada en: `[URL_DE_LA_APLICACIÓN]`

## Documentación

Para información técnica completa, consulta: [DOCUMENTACION_TECNICA.md](./DOCUMENTACION_TECNICA.md)

## Licencia

Este proyecto fue desarrollado como caso práctico para la asignatura de Interacción Hombre-Máquina.

## Autor

Desarrollado en 2024
