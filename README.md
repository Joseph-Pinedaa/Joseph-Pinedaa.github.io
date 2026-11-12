# Joseph A. Pineda — Engineering Portfolio

Live site: https://joseph-pinedaa.github.io

A plain HTML/CSS site with no build step, hosted on GitHub Pages. Every push to `main` goes live automatically.

## Structure

```
index.html                 home: intro + project cards
projects/                  one page per project
  seas.html
  motor-controller.html
  hercules-rocket.html
  training-app.html
  cnc-engraving.html
css/style.css
images/                    all photos go here
```

Each project page follows the same layout: **what it is and why → my role → tools → process (with images) → results / what's next.**
Each page opens with an image and a 2–3 sentence summary so recruiters can skim it, and the details are underneath.

## Adding photos

Gray dashed boxes marked **ADD PHOTO** are placeholders. To fill one:

1. Drop the image into `images/` (e.g. `images/hercules-build-1.jpg`). Keep files under ~500 KB. Resize phone photos first.
2. In the project page, replace the placeholder `<div class="ph">…</div>` with:
   ```html
   <figure><img src="../images/hercules-build-1.jpg" alt="Describe the photo"><figcaption>Caption</figcaption></figure>
   ```

## Rules to keep this repo safe (read before adding anything)

- **ESET 219 motor controller: no code or Quartus project files.** This is graded coursework. Post block diagrams, state diagrams and photos/video of it running on the board only. Never commit `.qpf`, `.qsf`, `.bdf`, `.v` or `.vhd` files from the lab.
- **SOMTECH / SEAS: ask Daniel Gambacorta before posting any code or detailed photos.** The team's repos are private. Describing your role is fine, and that's all the page does right now.
- **Training app / Supabase: never commit keys.** If you publish the app's repo, keep keys in a `.env` file (already in `.gitignore`). Never put the **service role key** anywhere in a frontend or public repo. The anon key is only OK on the frontend if Row Level Security is enabled on every table.
- **Keep it short and visual.** Each page should open with an image and a few sentences, with the deeper detail below.
- **Personal info:** the site lists your TAMU email and LinkedIn only. Don't post your resume PDF here unless you remove your phone number first, because this repo is public.
