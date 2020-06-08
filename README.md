# Stitches for tailblocks

A simple, fast web app to generate html based on a collection of commonly used user interface patterns.

Based on [Stitches](https://stitches.hyperyolo.com) and [tailblocks](https://mertjf.github.io/tailblocks/).

## 🎏 Live Site: []()

![app-screen-shot](https://cdn-images-1.medium.com/max/2000/1*DqVCpGnXJefwLXFneEHPZg.png)

## Running it locally

cd into Stitches directory.

```
npm install
```

Run Browserify to bundle all node modules.

```
browserify main.js -o bundle.js
```

Recompile tailwind css.

```
npx tailwind build stitches.css -c ./tailwind.config.js -o ./output.css
```

## Make your own templates

Feel free to take this project and re-factor to your need! Not everyone wants these templates for their projects. Here are the steps:

1. Run the project locally (see the section above)
2. Use [200 ok](https://chrome.google.com/webstore/detail/web-server-for-chrome/ofhbbkphhbklhfoeikjpcbhemlocgigb?hl=en) to run the repo in browser (because file download requires http).
3. Add your own HTML template (with tailwind.css classes) into the `templates` folder
4. Add a filter button for it in the `index.html`. (i.e. add `<button class="text-black font-semibold hover:text-green-500 px-2 py-1 transition-normal" data-filter="st-<your template name>">Tabs</button>`)
5. Done! refresh to check out your own templates.

## Contributing to the repo

I'll try to keep the templates up-to-date, feel free to issue pull requests if I'm slacking off 😁

## License

MIT © [Amie Chen](https://amie-chen.com) - Stiches Template Generator
MIT © [Mert Cukuren](https://mertjf.github.io/tailblocks/) - tailblocks Ready-to-use Tailwind Blocks
MIT © [Fabio Maienschein](https://maienschein.tech/) - putting those two together for simplicity
