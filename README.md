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

Search `index.html` for `FILM COUNTER`. Edit the three values on `#film-sqft`:

- `data-start-sqft` (`START_SQFT`) — total square feet on the start date
- `data-start-date` (`START_DATE`) — `YYYY-MM-DD`, midnight UTC
- `data-sqft-per-day` (`SQFT_PER_DAY`) — square feet added per day after that

The page shows `START_SQFT + time since START_DATE × SQFT_PER_DAY`. Everyone sees the same number, and it keeps ticking while the page is open. Also set the text inside the span to `START_SQFT` with commas, so visitors without JavaScript still see the starting total.

`START_SQFT` is 127,764 as of `2026-11-24`. `SQFT_PER_DAY` is 650. Both numbers are confirmed.

## Publish

Commit and push to `main`. GitHub Pages usually updates within a minute.
