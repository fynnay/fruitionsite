# Fruition: Free, Open Source Toolkit For Customizing Your Notion Pages

* Use cases: perfect for your portfolio, blog, landing page, and business site
* Features: pretty URLs, custom domains, Google Fonts, SEO support, script injection
* Benefits: completely free, no lock-in, and open source

For step-by-step setup instructions, visit https://fruitionsite.com

This repo has 2 independent parts:
1. [worker.js](https://github.com/stephenou/fruitionsite/blob/master/worker.js) is the Cloudflare Worker script
2. everything else is a React app that helps generate the Worker script via a UI.

## Notes

Snippets for modifying visuals of the site

### Custom buttons (from Super)

```css
<style>
	.notion-callout {
		border-radius: 100px !important;
		position: relative !important;
		padding: 16px 24px !important;
		border: none !important;
	}
	
	.notion-callout.bg-purple-light {
		box-shadow: 0 10px 20px -10px #516Bbef !important;
		background: #516bef !important;
	}
  
	.notion-callout.bg-yellow-light {
		box-shadow: 0 10px 20px -10px #f0bd66 !important;
		background: #f0bd66 !important;
	}
  
	.notion-callout.bg-blue-light {
		box-shadow: 0 10px 20px -10px #1ea1f1 !important;
		background: #1ea1f1 !important;
	}

	.notion-callout a {
		letter-spacing: -0.5px !important;
		padding: 0 0 2px 66px !important;
		align-items: center !important;
		position: absolute !important;
		font-weight: 600 !important;
		display: flex !important;
		border: none !important;
		color: #fff !important;
		bottom: 0 !important;
		right: 0 !important;
		left: 0 !important;
		top: 0 !important;
	}
</style>
```

