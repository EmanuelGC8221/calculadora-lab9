## 📌 Laboratorio 9 – Mezcla de ramas

Se continuó el desarrollo de la **calculadora**, implementando las siguientes funcionalidades:

| Funcionalidad | Rama creada |
|---------------|-------------|
| Restar dos números | `feature/operacion-resta` |
| Multiplicar dos números | `feature/operacion-multiplicacion` |
| Dividir dos números | `feature/operacion-division` |
| Calcular factorial | `feature/operacion-factorial` |
| Calcular exponente | `feature/operacion-exponente` |
| Calcular raíz cuadrada | `feature/operacion-raiz-cuadrada` |

Cada rama fue creada desde `develop`, se implementó la funcionalidad, se hicieron commits, y se realizó el merge hacia `develop`.
## Hacer cambios y registrar los commits.
- git add index.js
git commit -m "implementar función de resta"
# Volvemos a develop y fusionamos.
- git checkout develop
  git merge feature/operacion-resta.

## Sincronización local con remoto.
- Configurar remoto: git remote add origin https://github.com/usuario/repositorio.git
- Subir a la rama principal: git push -u origin main
- Actualizar cambios del remoto al local: git pull origin develop
- Subir todo el desarrollo al repo remoto: git push origin --all

## Retos Enfrentados.
Inicialmente se presentó el error "fatal: not a git repository", lo cual se solucionó inicializando el repositorio con git init en la carpeta a trabajar.

Al crear la primera rama apareció el error "fatal: not a valid object name: 'master'", lo que evidenció que se debe crear primero un commit inicial antes de crear ramas.

## Cosas aprendidas:
Importancia de mantener un flujo ordenado de ramas (main, develop, feature/*nombre de rama*) y las diferencias entre repositorio local y remoto.
