# Readme Sepinaco

Este repositorio esta pensado para replicar el framework SAP Composable storefront (SAP Spartacus) hecho en Angular.

Se usara NextJS y con la filosofia del framework SAP Spartacus, realizando las conexiones de datos a una BD local con Prisma o a un API REST Endpoint hecho con Nodejs y Express o con NestJS. Podremos elegir todas esas opciones.

Se podra reemplazar los componentes y las paginas de los que vienen por defecto en el framework.

Se usara como soporte el proyecto next-teslo-shop del curso de udemy de NextJS de Fernando Herrera. Asi tendremos un ejemplo real de e-commerce realizado con NextJS.

TODOS:

1) Crear pagina en framework (packages)
2) Usar pagina en example (apps)
3) Reemplazar pagina en example (apps)

1) Crear componente en framework
2) Usar componente en example
3) Reemplazar componente en example

1) Crear servicio en framework
2) Usar servicio en example
3) Reemplazar servicio en example

1) Usar storybook¿?

1) Usar Jest y testear Nextjs Framework

Arquitectura:

Escribir arquitectura de next-teslo-shop adaptada a mi arquitectura de nextjs sap composable storefront, con todos los archivos que necesito pero en carpetas organizadas de manera mas modular entiendo.

Crear package nuevo con nextjs: (https://turbo.build/repo/docs/crafting-your-repository/creating-an-internal-package
)
en donde voy a hacer el framework y despues en apps escribo las apps de pruebas y las de mis clientes que usaran el framework escrito en package/framework-next-sepinaco

Escribir el framework nextjs en packages/framework-next-sepinaco siguiendo los pasos https://turbo.build/repo/docs/crafting-your-repository/creating-an-internal-package

Usar el framework en los proyectos definidos dentro de la carpeta apps (como docs y web)

# Turborepo starter

This is an official starter Turborepo.

## Using this example

Run the following command:

```sh
npx create-turbo@latest
```

## What's inside?

This Turborepo includes the following packages/apps:

### Apps and Packages

- `docs`: a [Next.js](https://nextjs.org/) app
- `web`: another [Next.js](https://nextjs.org/) app
- `@repo/ui`: a stub React component library shared by both `web` and `docs` applications
- `@repo/eslint-config`: `eslint` configurations (includes `eslint-config-next` and `eslint-config-prettier`)
- `@repo/typescript-config`: `tsconfig.json`s used throughout the monorepo

Each package/app is 100% [TypeScript](https://www.typescriptlang.org/).

### Utilities

This Turborepo has some additional tools already setup for you:

- [TypeScript](https://www.typescriptlang.org/) for static type checking
- [ESLint](https://eslint.org/) for code linting
- [Prettier](https://prettier.io) for code formatting

### Build

To build all apps and packages, run the following command:

```
cd my-turborepo
pnpm build
```

### Develop

To develop all apps and packages, run the following command:

```
cd my-turborepo
pnpm dev
```

### Remote Caching

Turborepo can use a technique known as [Remote Caching](https://turbo.build/repo/docs/core-concepts/remote-caching) to share cache artifacts across machines, enabling you to share build caches with your team and CI/CD pipelines.

By default, Turborepo will cache locally. To enable Remote Caching you will need an account with Vercel. If you don't have an account you can [create one](https://vercel.com/signup), then enter the following commands:

```
cd my-turborepo
npx turbo login
```

This will authenticate the Turborepo CLI with your [Vercel account](https://vercel.com/docs/concepts/personal-accounts/overview).

Next, you can link your Turborepo to your Remote Cache by running the following command from the root of your Turborepo:

```
npx turbo link
```

## Useful Links

Learn more about the power of Turborepo:

- [Tasks](https://turbo.build/repo/docs/core-concepts/monorepos/running-tasks)
- [Caching](https://turbo.build/repo/docs/core-concepts/caching)
- [Remote Caching](https://turbo.build/repo/docs/core-concepts/remote-caching)
- [Filtering](https://turbo.build/repo/docs/core-concepts/monorepos/filtering)
- [Configuration Options](https://turbo.build/repo/docs/reference/configuration)
- [CLI Usage](https://turbo.build/repo/docs/reference/command-line-reference)




Textos antiguos =======================


1) carpeta docs: Contiene el proyecto NextJS de nuestro Framework (este proyecto usara la componentes visuales definidos en packages/ui, pero de momento defino los componenetes visuales en este proyecto de docs)
2) carpeta web: Contiene el proyecto NextJS que usa nuestro framework (proyecto especifico para un cliente)
3) carpeta packages/ui: Contiene la libreria de componentes que voy a crear y a usar en el framework (Aqui le pongo todo lo relacionado con r3f y componentes visuales que solo depende de los parametros que le pasemos)

NO: De momento escribire todo el codigo en docs, ahi hare un ecommerce y luego lo ire separando en packages/ui si eso.
NO: De momento voy a escribir todo el codigo que vaya a utilizar en los proyectos de mis clientes en packages/ui, y el ejemplo de como utilizarlo y conectarlo en el proyecto docs. Despues el proyecto web tendre que replicar lo que he hecho en docs y sera orientado para un cliente concreeto. Es decir, el proyecto docs es mi proyecto sucio de pruebas usando mi libreria packages/ui, el proyecto packages/ui es mi proyecto libreria framework e-commerce imitando a SAP-Spartacus, el proyecto web es el proyecto que imitiaria un proyecto a un cliente (posidonia shop o charles shop)
NO: En nuestro proyecto package/ui ponemos todo el codigo agnostico de framework o react (servicios con fetches, hooks, componentes, stores,...) (pero no ponemos codigo de Nextjs porque no vamos a incluir esa dependencia)

SI: Seguir las indicaciones de chatgpt para crear varios packages con nextjs y mis funcionalidades

https://turbo.build/repo/docs/crafting-your-repository/creating-an-internal-package

============