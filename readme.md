# Clean node

## Setup
  - git conventional 
    [https://www.conventionalcommits.org/en/v1.0.0/]
  - git commit msg linter
    - Um biblioteca q vai garantir o formato q no site acima
    - npm i git-commit-msg-linter
  - typescript
    - npm i -D typescript @types/node
    - create file `tsconfig.json`
  - eslint with typescript
    - npm install --save-dev \
  typescript@\* \
  eslint@^8.0.1 \
  eslint-plugin-promise@^6.0.0 \
  eslint-plugin-import@^2.25.2 \
  eslint-plugin-n@^15.0.0 \
  @typescript-eslint/eslint-plugin@^5.0.0 \
  eslint-config-standard-with-typescript@latest
    - create file `.eslint` vms dizer p ele q iremos usaor configs do `tsconfig.json`
    - comitar encima de um comite ja feito
      - Juntar no comite anterio 
      - git commit --amend --no-edit
    - husky permite ao nosso progeto definir hooks p nosso git
      - seria comando q podem ser executados antes da gente 
      - fazer um commit ou push
      - npm i husky -D 
        - create file `.huskyrc.json` 
        - temos um problema caso tenha muitos meninos p comitar
        - npm i -D lint-staged
          - ele permite q rodemos script somente em nosso stage areas
            - Ou seja rodar o script somente nos arqs modificados
            - create file `.lintstagedrc.json`
  - jest para teste
    - npm i -D jest @types/jest ts-jest
    - com ele instalado vamos criar o arq de configuracion
      - jest --init
        - [ yes, node, yes, no]
  - 


