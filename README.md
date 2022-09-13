# Craft + Storybook bootstrap

_A quick bootstrap for Storybook, for use alongside a Craft install._

Download these files and add to the root of an existing Craft CMS project. Probably best to start with an empty Craft install.

Run `npm i` to install the required files for Storybook. Then run `npm run storybook` to launch Storybook.

The example folder structure for template components and their corresponding `*.stories.js` files should be enough to get you going.

## Issues

Not all twig tags are supported with the twig package thats used to load twig templates within Storybook and complex components get more difficult to emulate within Storybook. The `/.storybook/preview.js` file allows some customisation for twig tags, but for some reason the available "extend" and "extendTag" functionality of twig simply do not want to work in the Storybook runtime.
