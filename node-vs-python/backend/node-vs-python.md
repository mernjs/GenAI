# **Node.js vs Python Setup Guide**

| Feature / Purpose                | **Node.js + Express + Prisma**                                                                  | **Python + FastAPI + SQLAlchemy**                                                                 |
| -------------------------------- | ----------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------- |
| **Language Runtime**             | `node`                                                                                          | `python`                                                                            |
| **Install (System-level)**       | - Download from [nodejs.org](https://nodejs.org) <br> - Or use `nvm` or system package managers | - Download from [python.org](https://python.org) <br> - Or use `pyenv` or system package managers |
| **Package Manager**              | `npm` (Node Package Manager)                                          | `pip` (Python Installer Package)                                                                  |
| **Init New Project**             | `npm init`                                                                       | Manual creation or use Poetry / `pipenv`                                                          |
| **Install Package (Local)**      | `npm install express prisma @prisma/client bcryptjs jsonwebtoken body-parser`                   | `pip install fastapi uvicorn sqlalchemy bcrypt pyjwt pydantic`                                    |
| **Install Package (Global)**     | `npm install -g nodemon`                                                                        | `pip install --user uvicorn`                                       |
| **Version Manager**              | `nvm` (Node Version Manager)                                                                    | `pyenv` (Python Version Manager)                                                                  |
| **Environment Management**       | `.nvmrc` + `nvm use`                                                                            | `venv`, `virtualenv`, `.python-version` with `pyenv`                                              |
| **Create Virtual Environment**   | Not common (Node uses global or project-level `node_modules`)                                   | `python -m venv env` <br> or `virtualenv env`                                                     |
| **Activate Virtual Environment** | N/A (not required for Node.js)                                                                  | `source env/bin/activate` (Linux/macOS) <br> `.\env\Scripts\activate` (Windows)                   |
| **Dependency Lock File**         | `package-lock.json` (yarn)                                               | `requirements.txt`, `Pipfile.lock`,                                             |
| **Scripts / Task Runner**        | Defined in `package.json` under `"scripts"`                                                     | Usually custom scripts, `Makefile`, or tools like `invoke`, `doit`, or `tox`                      |
| **Development Server (Common)**  | `nodemon index.js` or `node index.js`                                                           | `uvicorn main:app --reload`                                                                       |
| **Database ORM / Client**        | Prisma (`@prisma/client`)                                                                       | SQLAlchemy (Core + ORM)                                                                           |
| **Database Migration**           | `npx prisma migrate dev --name init`                                                            | SQLAlchemy auto-create tables via `Base.metadata.create_all(engine)`                              |
| **Password Hashing**             | `bcryptjs`                                                                                      | `bcrypt`                                                                                          |
| **JWT Authentication**           | `jsonwebtoken`                                                                                  | `pyjwt`                                                                                           |
| **Official Registry**            | [npmjs.com](https://www.npmjs.com)                                                              | [PyPI.org](https://pypi.org)                                                                      |

---

# **Notes for Both**

**Environment Management**

* Node.js: `.nvmrc` file + `nvm use`
* Python: `venv`, `.python-version` for pyenv

**Dependency Lock Files**

* Node.js: `package-lock.json` (npm) / `yarn.lock`
* Python: `requirements.txt`, `Pipfile.lock`, or `poetry.lock`

**Password Hashing**

* Node.js: `bcryptjs`
* Python: `bcrypt`

**JWT Authentication**

* Node.js: `jsonwebtoken`
* Python: `pyjwt`

**Development Server**

* Node.js: `node index.js` / `nodemon index.js`
* Python: `uvicorn main:app --reload`

---