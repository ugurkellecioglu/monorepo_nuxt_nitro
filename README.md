It's a monorepo powered by turborepo.

1. web folder contains a nuxt 3 app which has nitro server in it.
   go to /api/nuxt-endpoint to see the output

2. nitro folder has nitro server and it has a endpoint which returns a json.
   it runs on the edge see nitro.config.ts

here is how I tested it:

1. went to vercel and select the repository
2. some configuration needs to be done:
3. Framework presets: Nuxt JS
4. Root directory: edit > apps > web
5. build and output settings: override build command > "cd .. && pnpm run build"
6. deploy
