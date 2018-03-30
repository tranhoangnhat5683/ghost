#Clone source
```bash
git clone https://github.com/tranhoangnhat5683/ghost.git
```
or
```bash
git clone git@github.com:tranhoangnhat5683/ghost.git
```
#Install project
```bash
cd ghost
npm install
cp core/server/config/env/template.config.development.json core/server/config/env/config.development.json
vi core/server/config/env/config.development.json
cp core/server/config/env/template.config.production.json core/server/config/env/config.production.json
vi core/server/config/env/config.production.json
npm install -g knex-migrator
knex-migrator init
node index.php
```
#Setup env
Chose one env.
```bash
export NODE_ENV=development
export NODE_ENV=production
```
