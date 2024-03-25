# docs.*
Repository to centralize Projects, Issues and things cross all docs.* repositories.

## Repositories
- [docs.extractor](https://github.com/clj-codes/docs.extractor) -  Tool to extract namespace/functions documentation from Clojure projects into indexed Datalevin file. 
- [docs.backend](https://github.com/clj-codes/docs.backend) -  Backend Service for docs.clj.codes 
- [docs.frontend](https://github.com/clj-codes/docs.frontend) - Frontend SPA for docs.clj.codes

## Projects
- [Next Steps Kanban](https://github.com/orgs/clj-codes/projects/2)

## Using the project

### Configuration
Here some documentation about how to configure the repositories:
- [docs.extractor](https://github.com/clj-codes/docs.extractor?tab=readme-ov-file#config-resourcesconfigedn) -  Definitions of where to store the database and which libraries to analyze and index 
- [docs.backend](https://github.com/clj-codes/docs.backend?tab=readme-ov-file#config-resourcesconfigedn) -  Webserver, Database and Github api configurations
- [docs.frontend](https://github.com/clj-codes/docs.frontend?tab=readme-ov-file#config-srccodescljdocsfrontendconfigcljs) - Base backend url and github client for login

### How to use
After configuring the repositories you can run the database extraction on `docs.extractor`, then copy the resulting files inside the `docs.backend` (you can configure the url auto download in the config) and 
start it together with the `docs.frontend`.

Today I use [fly.io](https://fly.io) on [docs.clj.codes](https://docs.clj.codes/) to deploy this setup you can check the Github actions deploy files ([backend](https://github.com/clj-codes/docs.backend/blob/main/.github/workflows/flyio-deploy.yml), [frontend](https://github.com/clj-codes/docs.frontend/blob/main/.github/workflows/flyio-deploy.yml)) for some inspiration.

This setup is costing only $5/month currently:
<img width="735" alt="image" src="https://github.com/clj-codes/docs/assets/1683898/f0b399e1-08de-437f-b53b-b67e3b6f3ef3">
