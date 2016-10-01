# Use nodemon to run specs automatically on each save
- `npm install nodemon -g` - globally installs the nodemon module from npm
- `nodemon --exec "jasmine-node .`

Now when you save, it should automatically run `jasmine-node .`.

Make sure you're in the corresponding directory.
