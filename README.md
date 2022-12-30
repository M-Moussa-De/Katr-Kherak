# Katr Kherak (may ALLAH increase your well-being)

It's a full stack project running throughout the <span style="background: #eee;">SDLC</span> for the <span style="background: #eee;">"software development process" and the UML/OOP courses Of the Software Engineering Diploma 2022/2023 at the Cairo university</span>.

It's a non-profit, charitable organization that distributes food to those who have difficulty purchasing enough to avoid hunger.

The project follows the Minimum Viable Product (MVP). The key premise behind the idea of MVP is producing an actual product or a service, that you can offer to customers and observe their actual behavior with the product. Seeing what people actually do with a product is much more reliable than asking people what they would do.

## The idea behind the project

The main goal from the beginning of this idea was how to eradicate hunger and provide food for people residing in the same surrounding geographical area.
The food it will be first phase, but the next phase will be adding another category like provide medication that excess or unused.

We should do it out of social and religious motivation and moral, because if we are not going to do that for those reasons, then it is also in your national security and financial interest because if you do not, it will cost you a thousand times more in the long run.
Provide food will be made a friendly relationship & benevolent between the surrounding neighbors
As well as to preserve the environment and reduce food waste.

## Getting started

To have the project running locally, you need Node installed on your machine. This will allow you to use the npm to run commands in the terminal.
You can check if it installed by hitting this command `node -version` either you get the installed version and then you can go further with the steps below.
However, if you see an error, this means you should install [Node](https://nodejs.org/en/download/) from their official website according to your OS and you should consider installing the LTS version.

Now, open your terminal/shell of your choice (The integrated terminal within the VS Code will do the job :slightly_smiling_face:) and follow these steps respectively:

1. Run this command `npm git clone https://github.com/M-Moussa-De/Katr-Kherak.git` to clone the repository or you can download it as zip.

2. Run `npm install` to install the dependencies.

3. Run this command `npm run dev` to have it running locally in the development mode.

### Possible problems while trying to run the repo locally

When running the `npm run dev`, you might encounter an error like "Error: error:0308010C:digital envelope routines::unsupported".

This is happening properly because you're not using the LTS (long term support) version of Node JS.

A way to get around it, is to run in your terminal this command `export NODE_OPTIONS=--openssl-legacy-provider`

and after that run the `npm run dev` and it should work poperly.

## The used technologies

- Front-End

  - HTML
  - CSS
  - SASS
  - Vue JS
  - Nuxt JS
  - Bootstarp Vue

- Back-End

  - C#
  - .Net Core
  - SQL Server

- Documentaion

  - Lucidchart to create the different types os diagrams

## Diagrams

Within the diagrams folder, there're different type of diagrams, we build them during the Requirement analysis phase. You might like to have a look
To get the project structure easily.

#### Have you encountered any unexpected behaviors or errors, please, do not hesitate to contact us.
