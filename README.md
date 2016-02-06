# mytodo

This project is generated with [yo angular generator](https://github.com/yeoman/generator-angular)
version 0.15.1.

## Build & development

Run `grunt` for building and `grunt serve` for preview.

## Testing

Running `grunt test` will run the unit tests with karma.

# MY NOTES
## start with generator-angular

```
node --version && npm --version && git --version
npm install --global yo bower grunt-cli
yo --version && bower --version && grunt --version

npm install --global generator-angular generator-karma

mkdir mytodo && cd mytodo
yo angular

grunt serve
```

## to production

```
grunt
grunt serve:dist

scp -R dist ssh://remoteserver:/
```

dist in git
```
git add dist && git commit -m "Initial dist subtree commit"
git subtree push --prefix dist origin gh-pages

now, to deploy the dist directory, you have always run
git subtree push --prefix dist origin gh-pages
```
