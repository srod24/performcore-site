# PerformCore website

Public site for PerformCore (Perform Core Group), window film and tint in Naples, Florida. The company serves Collier and Lee counties.

The live site is [https://performcoregroup.com/](https://performcoregroup.com/). GitHub Pages publishes the `main` branch, so merging to `main` updates the live site.

Do not edit `CNAME` or the GitHub Pages domain settings unless you mean to move the domain.

## Update the phone number

Edit the `PERFORMCORE` block near the top of `index.html`:

```js
phone: "(239) 296-9853",
phoneTel: "+12392969853"
```

That block updates the call buttons, the phone lines in the page, and the LocalBusiness schema telephone.

## Update square feet of film applied

Search `index.html` for `FILM COUNTER`. Change only the text inside the element with id `film-sqft`.

- A whole number, such as `250000` or `250,000`, counts up when the stat scrolls into view.
- If the visitor has reduced motion turned on, the final number appears right away.
- Anything that is not a whole number is shown exactly as typed, including the `XXXXXXXXX` placeholder. The page will not show `NaN`.

## Publish

Commit and push to `main`. GitHub Pages usually updates within a minute.
