# vite-start-PoC

Vite init, repositorio destinado a poder comprender como se puede implementar vite en un proyecto y cual es su configuracion

Comandos a utilizar:
pnpm init (segun el gestor de paquetes)
pnpm create vite // npm create vite@latest
Seleccionamos con la navegacion proporcionada luego del comando,
En nuestro caso, React, Typescript y eslint.
Se nos crea la carpeta indicada con el nombre del proyecto, y un archivo vite.config.ts con la siguiente configuracion:

// defineConfig es una función de utilidad de Vite que proporciona autocompletado e InteleSense
import { defineConfig } from 'vite'

// Importamos el plugin oficial de Vite para React.
import react from '@vitejs/plugin-react'

// Exportamos la configuración usando defineConfig.
export default defineConfig({
// La propiedad 'plugins' acepta un arreglo de extensiones que modifican o amplían el comportamiento de Vite.
// Al ejecutar react(), se integran las herramientas para procesar JSX/TSX y habilitar Fast Refresh.
plugins: [react()],
})
