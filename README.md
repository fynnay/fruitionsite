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

### Custom Colors

```css
<style>
  :root {
    --color-bg-default: #000 !important;
  }
</style>
```

**All available colors**

```css
<style>
  :root {
    --color-text-default: #37352f;
    --color-text-default-light: rgba(55,53,47,0.6);
    --color-text-gray: #9b9a97;
    --color-text-brown: #64473a;
    --color-text-orange: #d9730d;
    --color-text-yellow: #dfab01;
    --color-text-green: #0f7b6c;
    --color-text-blue: #0b6e99;
    --color-text-purple: #6940a5;
    --color-text-pink: #ad1a72;
    --color-text-red: #e03e3e;
    --color-bg-default: #fff;
    --color-bg-gray: #ebeced;
    --color-bg-brown: #e9e5e3;
    --color-bg-orange: #faebdd;
    --color-bg-yellow: #fbf3db;
    --color-bg-green: #ddedea;
    --color-bg-blue: #ddebf1;
    --color-bg-purple: #eae4f2;
    --color-bg-pink: #f4dfeb;
    --color-bg-red: #fbe4e4;
    --color-bg-gray-light: rgba(235,236,237,0.3);
    --color-bg-brown-light: rgba(233,229,227,0.3);
    --color-bg-orange-light: rgba(250,235,221,0.3);
    --color-bg-yellow-light: rgba(251,243,219,0.3);
    --color-bg-green-light: rgba(221,237,234,0.3);
    --color-bg-blue-light: rgba(221,235,241,0.3);
    --color-bg-purple-light: rgba(234,228,242,0.3);
    --color-bg-pink-light: rgba(244,223,235,0.3);
    --color-bg-red-light: rgba(251,228,228,0.3);
    --color-pill-default: rgba(206,205,202,0.5);
    --color-pill-gray: hsla(45,2%,60%,0.4);
    --color-pill-brown: rgba(140,46,0,0.2);
    --color-pill-orange: rgba(245,93,0,0.2);
    --color-pill-yellow: rgba(233,168,0,0.2);
    --color-pill-green: rgba(0,135,107,0.2);
    --color-pill-blue: rgba(0,120,223,0.2);
    --color-pill-purple: rgba(103,36,222,0.2);
    --color-pill-pink: rgba(221,0,129,0.2);
    --color-pill-red: rgba(255,0,26,0.2);
    --color-ui-hover-bg: rgba(55,53,47,0.08);
  }
</style>
```
