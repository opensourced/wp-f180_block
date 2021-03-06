# Faculty 180 Gutenberg Block
### Integrate Interfolio's Faculty 180 product with WordPress

The following *must* be defined in your wp-config:

```
define('INTERFOLIO_PUBLIC_KEY', '<puclic-key>');
define('INTERFOLIO_PRIVATE_KEY', '<private-key>');
define('INTERFOLIO_DATABASE_ID', '<database-id>'); 
```
	
The URL for the Interfolio Faculty 180 API is already set to "https://faculty180.interfolio.com/api.php".  This can be overridden by defining `'INTERFOLIO_HOST'` in your wp-config file.

Display formats are defined in src/block/formats.js.  A default format is provided, along with an example section-specific format.

Sections you don't want to be available for display can be set in [src/block/config.js](https://github.com/Tulane/wp-f180_block/blob/master/src/block/config.js).

**

This project was bootstrapped with [Create Guten Block](https://github.com/ahmadawais/create-guten-block).

Here's information on how to run scripts:

### 👉  `npm start`
- Use to compile and run the block in development mode.
- Watches for any changes and reports back any errors in your code.

### 👉  `npm run build`
- Use to build production code for your block inside `dist` folder.
- Runs once and reports back the gzip file sizes of the produced code.

### 👉  `npm run eject`
- Use to eject your plugin out of `create-guten-block`.
- Provides all the configurations so you can customize the project as you want.
- It's a one-way street, `eject` and you have to maintain everything yourself.
- You don't normally have to `eject` a project because by ejecting you lose the connection with `create-guten-block` and from there onwards you have to update and maintain all the dependencies on your own.

>You can find the most recent version of this guide [here](https://github.com/ahmadawais/create-guten-block).
