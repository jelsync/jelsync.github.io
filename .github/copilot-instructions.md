# Guía para AI Agents - Portafolio de Jelsyn Ceron

## Descripción General

Este es un portafolio personal y CV de Jelsyn Johan Ceron Alvarez, desarrollador backend con experiencia en microservicios, Java Spring Framework, Docker, Kubernetes y DevOps.

## Estructura del Proyecto

```
.
├── index.html                   # Página principal (CV + Portafolio)
├── README.md                    # Documentación del proyecto
├── .github/
│   └── workflows/
│       └── deploy.yml           # GitHub Actions - Deploy automático
```

## Stack Tecnológico

- **Frontend:** HTML5, CSS3, JavaScript (Vanilla)
- **Despliegue:** GitHub Pages
- **CI/CD:** GitHub Actions
- **Librerias Externas:** html2pdf.js (para exportar PDF)

## Características Clave

1. **CV Descargable:** Botón para descargar el CV en PDF usando html2pdf.js
2. **Diseño Responsivo:** Media queries para impresión y dispositivos móviles
3. **Despliegue Automático:** GitHub Actions despliega automáticamente en GitHub Pages al hacer push

## Secciones del CV

- Información de contacto (Email, LinkedIn, GitHub)
- Resumen profesional
- Experiencia laboral
- Stack técnico (inferido de experiencia)
- Información de educación

## Patrones y Convenciones

- **Colores:** Azul corporativo (#2980b9) para enlaces y encabezados
- **Fuente:** Arial como fuente principal (segura y legible)
- **Espaciado:** Máximo 900px de ancho para mejorar legibilidad
- **Print-friendly:** CSS especial para impresión (color blanco, sin sombras)

## Flujo de Despliegue

1. Hacer cambios locales en index.html
2. `git add .` y `git commit`
3. `git push` a rama main/master
4. GitHub Actions ejecuta automáticamente el workflow de deploy
5. Cambios disponibles en `https://jelsync.github.io` (2-3 minutos)

## Comandos Comunes

```bash
# Clonar el repositorio
git clone https://github.com/jelsync/jelsync.github.io
cd jelsync.github.io

# Hacer cambios y desplegar
git add .
git commit -m "Descripción de cambios"
git push origin main
```

## Configuración de GitHub Pages

- **Repository:** jelsync.github.io
- **Source:** Deploy from a branch (main/master)
- **Folder:** / (root)
- **Domain:** jelsync.github.io

## Consideraciones Importantes

1. El archivo `deploy.yml` puede necesitar ajustes si el repositorio no se llama `jelsync.github.io`
2. La propiedad `cname` en deploy.yml debe coincidir con el nombre del repositorio
3. GitHub Pages requiere que el repositorio sea público para sitios de usuario
4. Los cambios pueden tardar 2-3 minutos en ser visibles después del push

## Próximas Mejoras (Opcionales)

- Agregar sección de proyectos destacados
- Implementar modo oscuro con CSS variables
- Agregar animaciones suaves con CSS
- Crear página separada para portfolio/proyectos
- Integrar formulario de contacto (con servicio como Formspree)

## Referencias

- [GitHub Pages Documentation](https://pages.github.com/)
- [HTML2PDF.js Documentation](https://ekoopmans.github.io/html2pdf.js/)
- [GitHub Actions for GitHub Pages](https://github.com/peaceiris/actions-gh-pages)
