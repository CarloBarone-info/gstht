# Divisional Rollup — interactive UX prototype

A deliberately low-fidelity, static demonstration of the design in the presentation (slides 6–8).

## Walkthrough aligned to the slides

1. **Payments division:** 5,000 pipelines → **100 failed**, 4,700 succeeded, 200 not run yet. Headline: **Failures detected**.
2. **Team overview:** Orders 16/180 (8.9%), Risk 22/320 (6.9%), Payments Ops 25/500 (5.0%), Insights 12/400 (3.0%), Ledger 12/700 (1.7%), Identity 7/600 (1.2%), Platform 4/1,200 (0.3%), Archive 2/1,100 (0.2%). Sorted by failure percentage, **not business severity**.
3. **Orders team:** 16 failed, 156 succeeded, 8 not run yet.
4. **Individual pipeline:** Select **orders-daily-export** → Failed → owning team **Orders**.

All data is fictional. Individual pipeline rows are **illustrative samples**, not a full listing of the 180 Orders pipelines. The page is not a production monitor.

## Run the GitHub Pages prototype locally

**No install or build required.** Clone the repo and open `docs/index.html` in a browser, or run a tiny local web server:

```bash
git clone https://github.com/CarloBarone-info/gstht.git
cd gstht
python3 -m http.server 8000 --directory docs
```

Visit **http://localhost:8000**. On Windows, `py -m http.server 8000 --directory docs` is an alternative.

**Note:** `npm install && npm run dev` launches the repository's *separate, pre-existing React/Vite scaffold*, not the static Pages prototype. You do not need npm for the site in `docs/`.

## Publish on GitHub Pages

1. Open **https://github.com/CarloBarone-info/gstht/settings/pages**.
2. Under **Build and deployment**, choose **Deploy from a branch**.
3. Choose branch **main**, folder **/docs**, then **Save**.
4. Allow several minutes for publication, then visit **https://carlobarone-info.github.io/gstht/**.

I cannot enable GitHub Pages settings through the available GitHub connector; the owner must do that step.

## Deliberate omissions

- No backend, auth, monitoring API, incident notifications or severity scores
- No unverified business-health grades or timestamps
- No assumption that "not run yet" is healthy or failed

## Privacy

GitHub Free supports Pages from **public repositories**. Changing the repository to **private** on Free will unpublish the site. A publicly published Pages site is not private even when the underlying repository is on an eligible paid plan.
