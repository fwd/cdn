![line](https://github.com/fwd/n2/raw/master/.github/line.png)

<h1 align="center" style="font-size: 30px">Simple Website Template</h1>
<h3 align="center" style="font-size: 30px">(HTML + Vue2 + Github Pages)</h3>

![line](https://github.com/fwd/n2/raw/master/.github/line.png)

**index.html**

```html
<!DOCTYPE html>
<html>
    <head>
		<title>Hello World</title>
		<meta name="apple-mobile-web-app-title" content="Hello World">
		<meta name="viewport" content="width=device-width, initial-scale=1">
		<meta name="apple-mobile-web-app-capable" content="yes">
		<meta name="apple-mobile-web-app-status-bar-style" content="black">
		<link rel="apple-touch-icon" href="/icon.png">
        <script src="https://cdn.fwd.dev/vue.js"></script>
        <script src="https://cdn.fwd.dev/axios.js"></script>
        <style>
            * { 
            	margin: 0; 
            	padding: 0; 
            	box-sizing: 
            	border-box; 
            }
        </style>
    </head>
    <body>
        <div id="app">
            {{ message }}
        </div>
        <script>
	        var app = new Vue({
				el: '#app',
				data: { 
					message: 'Hello World' 
				},
				mounted() {
					this.load()
				},
				watch: {},
				computed: {},
				methods: {
					load() {
						console.log("Ready!")
					}
				},
			})
        </script>
    </body>
</html>
```

## Github Pages

- Github repo must be public
- Go to [Settings Page](/../../settings/pages)
- Source → "Master" → "/Root"
- Save

Your public URL: https://NAME.github.io/REPO

## Custom Domain (Optional):

- Go to [Settings Page](/../../settings/pages)
- "Custom domain" → "Add Domain"
- Save

## Domain DNS Settings

- Create **A** record that points to: **185.199.108.153**
- If using Cloudflare, make sure to disable proxy.

Official Docs: https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site
