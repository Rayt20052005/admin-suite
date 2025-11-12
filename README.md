```
adminsuitex/
├── scripts/
│   └── menu.sh
│   └── red.sh
│   └── personas.sh
│   └── copias.sh 
│   └── logs.sh
│   └── sistema.sh
│
├── proyecto/
│   └── copias/ 
    └── reportes/
```
## Entorno de pruebas:
El script fue desarrollado y testeado en CentOS 7.

## Requisitos previos:
- Distribución Linux (CentOS 7+, Rocky, Alma, u otras distribuciones basadas en Red Hat).
- Acceso administrativo (sudo).
- Carpeta /home/ en el directorio raíz con permisos adecuados.

## Instalación normal:
1. Copiar la carpeta home a /.
2. Dar permisos de ejecución:
-- chmod +x menu.sh *.sh
3. Ejecutar el menú principal:
-- bash menu.sh

## Instalación en VM:
- Tener instalado el programa Oracle VirtualBox.
- Descargar e importar el archivo .ova correspondiente.
- Entrar a la configuración de la máquina virtual mientras esté apagada, ir a la sección de Red y habilitar los adaptadores necesarios.
- En cada uno, establecer el modo Adaptador puente para asegurar que no hayan fallos.
- Finalmente, iniciar la máquina virtual.

## Credenciales de la VM:
- Usuario: root
- Contraseña: abc123

## Uso básico:
- El menú principal muestra las partes principales del sistema.
- Cada submenú hace tareas específicas y guarda un registro de lo que se hizo en /var/log/adminsuite.log.

## Seguridad y buenas prácticas:
- No guardar contraseñas dentro de los scripts.
- Ejecutar siempre con permisos mínimos.
- Verificar la existencia de respaldos antes de restaurar.
 ```
