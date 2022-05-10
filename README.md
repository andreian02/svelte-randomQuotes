# Basic Random Quotes Generator made with Svelte

This serves as a basic random quotes generator app made with Svelte. <br>
The inital original workings to this is from [Build a Random Quote Machine with Svelte and Parcel
](https://dev.to/ringmaster/build-a-random-quote-machine-with-svelte-and-parcel-4l4c)

A transition effect was added as a feature the "share to tweet" was removed. <br>
Additional requirement installed is the [rollup/plugin-json](https://www.npmjs.com/package/@rollup/plugin-json).

---

## Get started

Git clone and run it with your own favourite quotes!

```bash
* git clone //this project
* npm i // npm install
* npm run dev // localhost:8080
```

Navigate to [localhost:8080](http://localhost:8080). You should see your app running. Edit a component file in `src`, save it, and reload the page to see your changes.

By default, the server will only respond to requests from localhost. To allow connections from other computers, edit the `sirv` commands in package.json to include the option `--host 0.0.0.0`.

If you're using [Visual Studio Code](https://code.visualstudio.com/) we recommend installing the official extension [Svelte for VS Code](https://marketplace.visualstudio.com/items?itemName=svelte.svelte-vscode). If you are using other editors you may need to install a plugin in order to get syntax highlighting and intellisense.

## Preview

![image](https://user-images.githubusercontent.com/36339564/167565798-d91e8dcc-45a3-4d5a-9a9e-f6eb00b8b5ef.png)

## Building and running in production mode

To create an optimised version of the app:

```bash
npm run build
```

You can run the newly built app with `npm run start`. This uses [sirv](https://github.com/lukeed/sirv), which is included in your package.json's `dependencies` so that the app will work when you deploy to platforms like [Heroku](https://heroku.com).

## Deploying to the web

### With [Vercel](https://vercel.com)

Install `vercel` if you haven't already:

```bash
npm install -g vercel
```

Then, from within your project folder:

```bash
cd public
vercel deploy --name my-project
```
