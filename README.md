**Autor:** Juan Carlos Luna  
**Versión:** 1.0

# Repositorio para Práctica de Resolución de Conflictos

En este repositorio se resolvieron problemas de colaboración con otros compañeros. Al trabajar en el mismo archivo y realizar un *push*, surgieron conflictos. 

La solución consistió en revisar los mensajes de error, ejecutar los comandos sugeridos y luego analizar manualmente los conflictos en los archivos. Posteriormente, añadimos los archivos al área de preparación, realizamos el *commit* para registrar los cambios, y al hacer un nuevo *push*, esta vez no obtuvimos ningún error.

## Uso de Este Repositorio para la Práctica de GitHub Pages y Jekyll

Este repositorio se ha utilizado para llevar a cabo la práctica de configuración de **GitHub Pages** y para implementar **Jekyll** en el despliegue del sitio web.

## Implementacion de un theme jekyll para el repositorio 
# Proyecto de GitHub Pages con el Tema Cayman

Mi repositorio utiliza el tema **Cayman** para GitHub Pages, proporcionando un diseño limpio y funcional para la presentación del contenido.

## Uso del Tema Cayman
Para la implementación del tema he realizado los siguientes pasos trabajando en local:

### 1. Configuración del archivo `_config.yml`
Agregar las siguientes líneas al archivo `_config.yml`: (En caso de no existir este fichero se debe crear en la raiz)

```yaml
remote_theme: pages-themes/cayman@v0.2.0
plugins:
  - jekyll-remote-theme

```
### 2. Configuración o creación del Gemfile
## ¿Qué es un Gemfile?
El `Gemfile` es un archivo de configuración utilizado por Bundler, una herramienta para gestionar dependencias en proyectos de Ruby, incluyendo aplicaciones Jekyll. En este archivo, se especifican las gemas (librerías) que el proyecto necesita para funcionar, junto con las versiones deseadas. Al ejecutar el comando `bundle install`, Bundler lee el `Gemfile` y descarga las gemas requeridas, asegurando que el entorno de desarrollo esté configurado correctamente. Esto permite mantener las dependencias del proyecto organizadas y facilitar su instalación en diferentes entornos.

### Línea del theme para nuestro Gemfile:
``` source "https://rubygems.org"
   2   │ gem "github-pages", group: :jekyll_plugins ```
```
### 3. Instalación de dependencias
```
bundle install
```

  ### Prueba en local del theme jekyll:
    Levantamos un servidor jekyll en nuestro entorno local:
    ```
    bundle exec jekyll serve 
    ```
    
### 4. Push a nuestro repositorio remoto:
```git add <archivos>
git commit -m "Mensaje"
git push origin master```
```

### CONFIGURACIÓNES ADICIONALES
Agregar esta linea a nuestro css para trabajar con el theme: 
```@import "{{ site.theme }}";
// Aquí puedes agregar tu CSS personalizado ```
```

Y podremos comprobar que se ha levantado nuestro sitio github-pages con este theme jekylls.




