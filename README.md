This is a [Next.js](https://nextjs.org/) project bootstrapped with [`create-next-app`](https://github.com/vercel/next.js/tree/canary/packages/create-next-app).

## Getting Started

First, run the development server:

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
# or
bun dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `app/page.tsx`. The page auto-updates as you edit the file.

This project uses [`next/font`](https://nextjs.org/docs/basic-features/font-optimization) to automatically optimize and load Inter, a custom Google Font.

#Deploy via docker
#Log in Azure 
#Create a container registry with name nextjsdockeronazure
#Run below command to create image
docker build -t nextjsdockeronazure.azurecr.io/nextjsdockeronazure:latest .
#Push the image to registry
docker push nextjsdockeronazure.azurecr.io/nextjsdockeronazure:latest
#Run the container
docker run -d -p 3000:3000 nextjsdockeronazure.azurecr.io/nextjsdockeronazure:latest
