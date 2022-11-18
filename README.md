# dsmeta
React in FrontEnd with Backend in Java

# Checklist

## Design Figma

+ https://www.figma.com/file/PehiT8Dw4Lv5ioTSULZeRI/DSMeta3
+ https://www.figma.com/file/Yu2RHFmirHQ4BIVZM2XxY6/DSMeta2
+ https://www.figma.com/file/EN1zFtk4eY3Jgmpgi9YaMG/DSMeta1

## Ferramentas

+ Nodejs 16 e Yarn (vídeo: https://youtu.be/x5tgFTS-CYA )
+ STS (vídeo: https://youtu.be/TGQ0K9QsX88 )
+ VS Code
  - IntelliCode
  - ESLint
  - JSX HTML <tags/>
  
## Passo: criar projeto ReactJS
`yarn create vite frontend --template react-ts`

## Passo: criar projeto Spring Boot
+ Criar projeto Spring Boot no Spring Initializr com as seguintes dependências:
  - Web
  - JPA
  - H2
  - Security
+ Ajuste no arquivo pom.xml:
```
<plugin>
	<groupId>org.apache.maven.plugins</groupId>
	<artifactId>maven-resources-plugin</artifactId>
	<version>3.1.0</version><!--$NO-MVN-MAN-VER$ -->
</plugin>`
```

## Passo: salvar primeira versão no Github
```
git init
git add .
git commit -m "Project created"
git branch -M main
git remote add origin git@github.com:seuusuario/seurepositorio.git
git push -u origin main
```

## Passo: "limpar" o projeto ReactJS
Pegar o CSS: 
```
https://github.com/acenelio/dsmeta-css
```
+ COMMIT: Project clean

## Passo: Primeiro componente
Projeto HTML/CSS: https://github.com/acenelio/dsmeta-css
+ COMMIT: First component

## Passo: Outros componentes
+ COMMIT: Other components

## Passo: Datepicker
Documentação: https://github.com/Hacker0x01/react-datepicker
```
yarn add react-datepicker@4.8.0 @types/react-datepicker@4.4.2
```
```
import DatePicker from "react-datepicker";
import "react-datepicker/dist/react-datepicker.css";
```

```
<DatePicker
    selected={new Date()}
    onChange={(date: Date) => {}}
    className="dsmeta-form-control"
    dateFormat="dd/MM/yyyy"
/>
```

+ COMMIT: Datepicker

## Passo: React Hook useState para manter estado das datas
Macete para criar uma data de X dias atrás:
```
const date = new Date(new Date().setDate(new Date().getDate() - 365));
```
+ COMMIT: useState

