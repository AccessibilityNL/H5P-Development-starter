# H5P Development starter

## Requirements

- Nodejs with NPM

## Install

See: https://h5p.org/development-environment

0. NodeJS
1. `npm install`
2. Setup your PHP dev environment

  - Use MAMP, XAMP or other similar software to quickboot. Clone / install this project in the httdocs folder and start the server.

  > TODO: Use a container installation with Docker or similar software.

3. Start the dev server and install drupal and configure.

  > Start server for the contents of `drupal` dir, see notes for step 2

  > Follow drupal instructions


4. Enable H5P Dev mode:

  1. login to drupal dashboard
  2. go to modules panel
  3. scroll down to "other" section
  4. enable h5p Modules
  5. Configure h5p:

    1. Check options: "Enable H5P development mode" and "Enable library development directory (For programmers only)"

5. Go into development dir `cd drupal/sites/default/files/h5p/development`;

6. Start importing the H5P modules you wish to develop / improve by using H5P's cli tool.

  > Enter the command `npx h5p` to see a list of options. You will mostly use the h5p list and get commands to see what modules are available and to get them.

  > To enable and edit the modules you are required to import both the module and its editor equivalent to add interactive content with drupal.

  > EXAMPLE: `npx h5p get h5p-true-false`




## Development

### Symlinken

Link src packages to H5P/development folder `drupal/sites/default/h5p/development/libraries`
