# Sitio web del Grupo de trabajo COVID-19 de Tokio

![](https://github.com/tokyo-metropolitan-gov/covid19/workflows/production%20deploy/badge.svg)

[![Tokyo COVID-19 Task Force website](https://user-images.githubusercontent.com/1301149/75629392-1d19d900-5c25-11ea-843d-2d4376e3a560.png)](https://stopcovid19.metro.tokyo.lg.jp/)

### [日本語](./README.md) | English | [Spanish](./README_ES.md) | [Korean](./README_KO.md) | [Chinese (Taiwan)](./README_ZH_TW.md) | [Chinese (Simplified)](./README_ZH_CN.md) | [Vietnamese](./README_VI.md) | [Thai](./README_TH.md)


## Cómo Contribuir

Todas las contribuciones son bienvenidas.!
Por favor, consulte [Cómo contribuir](./.github/CONTRIBUTING_ES.md) para obtener más detalles.

## Código de Conducta

Por favor, consulte el [Código de conducta para desarrolladores](./.github/CODE_OF_CONDUCT_ES.md) para más detalles.

## Licencia
Este software se publica bajo la [licencia MIT](./LICENSE.txt).

## Para Desarrolladoras

### Cómo Configurar Entornos

- Versión requerida de Node.js: 10.19.0 o superior

**Use yarn**
```bash
# install dependencies
$ yarn install

# serve with hot reload at localhost:3000
$ yarn dev
```

**Use docker**
```bash
# serve with hot reload at localhost:3000
$ docker-compose up --build
```

### Detect procition/others environment (translate me!)

On the production environment, `'production'` is assigned to `process.env.GENERATE_ENV` variable, on the other case `'development'` is assigned to the variable.
Please use the variable to detect which enviroinment is used at the runtime.

### Implementación en entornos de preparación y producción

Cuando se actualiza la rama `master`, los archivos HTML se construirán automáticamente en la rama de `production`,
y luego el sitio de producción (https://stopcovid19.metro.tokyo.lg.jp/) también se actualizará.

Cuando se actualiza la rama `staging`, los archivos HTML se construirán automáticamente en la rama `gh-pages`,
  y luego el sitio de preparación (https://stg-covid19-tokyo.netlify.com/) también se actualizará.

Cuando se actualiza la rama `development`, los archivos HTML se construirán automáticamente en la rama` dev-pages`,
y luego el sitio de desarrollo (https://dev-covid19-tokyo.netlify.com/) también se actualizará.
