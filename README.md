# PerformCore website

Public site for PerformCore window film in Naples, Florida.

Live preview: https://srod24.github.io/performcore-site/

The custom domain performcoregroup.com is not pointed here yet. Do not add a CNAME file until DNS is ready.

## Update the phone number

Edit the `PERFORMCORE` block at the top of `index.html`:

```js
phone: "(239) 296-9853",
phoneTel: "+12392969853"
```

Then publish:

```bash
cd /workspace/performcore-site && git add index.html && git commit -m "Update phone" && git push
```

GitHub Pages usually updates within a minute.
