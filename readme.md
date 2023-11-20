Na pasta:
- npm init -y
- no package.json, no name, eu defino o nome do pacote (Padrão para ambos @ignite-ui/name)
- Por se tratar de um pacote, eu crio um index e exporto todos os arquivos para quando eu for exportar p/ fora, ficar mais fácil.
- Install os arquivos TS (npm i -D typescript) and (npx tsx --init)
- Install tsup -D p/ converter ts em JS
- No package.json eu crio dois scripts: 
  1 - "build": "tsup src/index.ts --format esm,cjs --dts" - Para build
  2 - "dev": "tsup src/index.ts --format esm,cjs --dts --watch" - Para monitorar alterações no pacote e gerar o build automaticamente