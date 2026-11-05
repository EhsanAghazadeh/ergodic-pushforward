# Project page: Ergodic Trajectory Design by Learned Pushforward Maps (NeurIPS 2026)

Static project page served with GitHub Pages at
https://ehsanaghazadeh.github.io/ergodic-pushforward/

Code: https://github.com/EhsanAghazadeh/uav_ot_cfm

## Publish
1. Create the GitHub repo `EhsanAghazadeh/ergodic-pushforward` (public, empty).
2. `git remote add origin git@github.com:EhsanAghazadeh/ergodic-pushforward.git && git push -u origin main`
3. Settings → Pages → Source: *Deploy from a branch*, Branch: `main`, folder `/ (root)`.

## Update links
The **Paper** button (`id="paper-link"` in `index.html`) points to arXiv (https://arxiv.org/abs/2605.13063).
Swap in the NeurIPS proceedings URL once it is available.

## Animation assets
`static/flow/*_frames.png` (grayscale sprite sheet, 61 frames, s = 0 → 1),
`*_target.png` and `*_meta.json` are produced by `make_flow_animation.py` in the
code repo (`sbatch scripts/run_flow_animation.sh`); the page colourises them
in the browser. `*.gif` is the fallback used when JavaScript or fetch is unavailable.
Preview locally with `python -m http.server` (opening the file directly
falls back to the GIF).
