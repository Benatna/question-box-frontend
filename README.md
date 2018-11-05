

# Benatna Frontend

This is the front-end single page application developed to accompany the Back End of a [Question Box](https://github.com/Benatna/question-box-backend) REST-like API designed to promote a peer-to-peer, culturally appropriate approach to Sex Education in Refugees and New Germans.

The front-end consist of a Single Page Application developed using Vue.JS with Progressive Web App implementations. It connects via Axios with the back-end and it implements several functionalities of Service Workers: Push Notifications, Caching, Offline Usage, and Installing on an Android Mobile Device.

## Table of Contents

- [Prerequisites](#prerequisites)
- [Getting Started](#getting-started)
- [Running tests](#running-tests)
- [Environment Variables](#environment-variables)
- [API End-Points](#api-end-points)
  - [Public Routes](#public-routes)
  - [Private Routes](#private-routes)
- [Multilanguage](#multilanguage)
- [Technology](#technology)
  - [Database](#database)
  - [Encryption](#encryption)
  - [Push Notifications](#push-notifications)
  - [Email Notifications](#email-notifications)
- [Get in Touch](#get-in-touch)
- [Acknowledgements](#acknowledgements)
- [Team](#team)
- [License](#license)
- [Funding](#funding)

## Prerequisites

The back-end requires you to have **node.js ^8.10** and **npm ^3.5.2** installed in your development machine. The compiled minified version can run in any HTML server.

## Getting Started

First, download or clone this repository.

```
git clone https://github.com/Benatna/question-box-frontend.git
```

After downloaded, access the downloaded folder and install the required dependencies.

```
cd question-box-backend
npm install
```

You will also want to modify the environment variables files before using it.

```
nano .env
```

You can see the list of required environment variables and their definition [here](#environment-variables).

Once you have defined the environment variables, you can run the application using one of these three commands:

First, you can compile it and enable hot-reloading for development purposes:

```
npm run serve
```

Second, you can compile it and minify it for production:

```
npm run build
```

> **NOTE:** This will generate a "dist" folder that can be copied and run in any HTML server. If you want to test these files, you can do so using a package like [serve](https://www.npmjs.com/package/serve).

Finally, you can also run the included linter to fix some problems with the code:

```
npm run lint
```

## Environment Variables

| Variable        | Example   | Comments  |
| --------------- |---------------| ---------|
|VUE_APP_I18N_LOCALE| `VUE_APP_I18N_LOCALE=en` | Defines the initial language of your application (for when an user logins for the first time) |
| VUE_APP_I18N_FALLBACK_LOCALE | `VUE_APP_I18N_FALLBACK_LOCALE=en` |   If enabled, when a translation is not found, the version of this locale will be shown |
| VUE_APP_REST_API | `VUE_APP_REST_API=HTTP://API.YOURDOMAIN.COM/` | URL where your API is found. |
| VUE_APP_VAPID_PUBLIC_KEY | `VUE_APP_VAPID_PUBLIC_KEY=BCv-0bxPV_RQj(..)` | Generated VAPID public key. You can find more information about this on the [backend page](https://github.com/Benatna/question-box-backend) |

## Project Structure

The project is using Vue's component-based structure. We try to keep Javascript and CSS files ordered in such a way that if a class/function is implemented in multiple components, then it belongs to the parent component. You can find more information in [Vue.js official guide[(https://vuejs.org/v2/guide/components.html).

## Multilanguage

At the moment, language options are hard-coded, and implemented using the [Vue CLI 3 i18n plugin](https://github.com/kazupon/vue-cli-plugin-i18n). In the folder `/src/locales/` you can find two JSON files that are used for translation. You can modify existing text and/or add new text in these files. For more information, visit visit the [plugin's official page](https://kazupon.github.io/vue-i18n/).

## External Resources
- This project implements [Google Noto fonts family](https://www.google.com/get/noto/). Text is Noto Sans and Emojis are Noto Emoji.
- Footer icons based on [Google Material Icons](https://material.io/tools/icons/).
- About photo is public domain by [Alexis Brown](https://unsplash.com/photos/-Xv7k95vOFA?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText) on [Unsplash](https://unsplash.com/search/photos/diverse-teens?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText).

## Get in Touch

If you need any help and/or want to get in touch with us, don't hesitate to [Submit an Issue](https://github.com/Benatna/question-box-frontend/issues), and/or contact us at [contact@benatna.de](mailto:contact@benatna.de), or via [Facebook](#) and [Twitter](#).

## Acknowledgements

Thanks to Ahmad, Ahmed, Nickhil, Zain and Zeina for their support, hard work, and insights during the development and deployment of this solution.

## Team

This project was created in six months for the beautiful team of:

- **Cornelia Blum**: Lead.
- **Pedro Poblete Lasserre**: Coder.
- **Hector Pahaut**: Designer.
- **Pooja  Veerappa**: User Researcher.
- **Juli Maier**: Mentor.

## License

This project is licensed under the MIT License - see the  [LICENSE](https://github.com/Benatna/question-box-backend/LICENSE)  file for details.

## Funding

Funding for the initial development of this project came from the [Prototype Fund](https://prototypefund.de/), an initiative of the [German Federal Ministry of Education and Research](http://bmbf.de/).
