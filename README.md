---
---

# Gatsby Use sitemetada

#### GUS _by [Edu4Dev](https://edu4.dev)_

---

Shortcut to request business data written on `gatsby-config.js` siteMetadata.


## 🚀 Quick start

To get started to log data on your build, you can follow these steps:

1. Install Gatsby Use siteMetadata gatsby-plugin with the follow command:

```shell
npm i gatsby-use-sitemetadata
```

## 🧐 What's inside?

This plugin generates the [files Gatsby looks for inside node_modules](https://www.gatsbyjs.com/docs/files-gatsby-looks-for-in-a-plugin/).

	/gatsby-use-sitemetadata

	├── src/tools

	├────── useSitemetaData.js

	├── LICENSE(0BSD)

	├── package.json

	└── README.md


2. Plug and Play

There's no need to configure the plugin, just plug-n-play inside your custom block:

```javascript

import { useSiteMetadata } from 'gatsb-use-sitemetadata'

const MyAwesomeComponent = ({subAgent}) => {
	return <p>{useSiteMetadata.message}</p>
}

export default MyAwesomeComponent

```

Here is the query you're requesting for:

```graphql
query {
	site {
		siteMetadata {
			title
			headline
			basePath
			name
			version
			developer
			coauthorBusiness
			project
			url
			message
		}
	}
}
```

3. Verify the plugin was added correctly

If the plugin aren't working Gatsby will break.

## 🎓 Learning Gatsby

If you're looking for more guidance on plugins, how they work, or what their role is in the Gatsby ecosystem, check out some of these resources:

- The [Creating Plugins](https://www.gatsbyjs.com/docs/creating-plugins/) section of the docs has information on authoring and maintaining plugins yourself.
- The conceptual guide on [Plugins, Themes, and Starters](https://www.gatsbyjs.com/docs/plugins-themes-and-starters/) compares and contrasts plugins with other pieces of the Gatsby ecosystem. It can also help you [decide what to choose between a plugin, starter, or theme](https://www.gatsbyjs.com/docs/plugins-themes-and-starters/#deciding-which-to-use).
- The [Gatsby plugin library](https://www.gatsbyjs.com/plugins/) has over 1750 official as well as community developed plugins that can get you up and running faster and borrow ideas from.
