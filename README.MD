Repositorio del taller:

# Git hooks

En git hay una utilidad llamada githooks que nos permite ejecutar scripts antes de realizar una determinada acción, los hooks están disponibles para el cliente y para el servidor

Pero para lo que vamos a necesitar en general nos fijamos solo en los siguientes hooks que se ejecutan en el cliente:

## pre-commit
Este hook es el primero en ejecutarse, y sirve para comprobar la instantánea que vas a confirmar, puede ser útil para ejecutar las pruebas, o los lint, antes de commitear la instantánea, si falla esta el commit será cancelado.

## commit-msg
Este evento es lanzado cuando se guarda el mensaje del commit, y recibe el mensaje de ese commit, por lo que nos puede ser útil para aplicar algún lint sobre el mensaje, como asegurarnos que cumple una guía de estilos que tiene el identificador de la issue, entre otros.

# Enlaces de interes

* [husky](https://www.npmjs.com/package/husky)
* [lint-staged](https://www.npmjs.com/package/lint-staged)
* [@commitlint/cli](https://www.npmjs.com/package/@commitlint/cli)
* [@commitlint/config-conventional](https://www.npmjs.com/package/@commitlint/config-conventional)
* [standard-version](https://www.npmjs.com/package/standard-version)
* [Especificacion conventional commits](https://www.conventionalcommits.org/en/v1.0.0/)
* [Git Hooks](https://git-scm.com/book/es/v2/Personalizaci%C3%B3n-de-Git-Puntos-de-enganche-en-Git)