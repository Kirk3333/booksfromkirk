# Kirk Johnson — Author Website

A simple, fast website built with plain HTML and CSS. No build tools needed —
it works out of the box with GitHub + Netlify.

## What's in this folder

| File | What it is |
|---|---|
| `index.html` | Home page with all six books and Buy on Amazon buttons |
| `about.html` | About page (edit the bio — look for the EDIT YOUR BIO HERE comment) |
| `specials.html` | Free first chapter offer with email signup form |
| `contact.html` | Contact form + your email (kirkinphx@gmail.com) |
| `thanks.html` | Thank-you page shown after someone submits a form |
| `css/style.css` | All the styling for the whole site |
| `images/` | Your six book covers |

## How to put this site online (one-time setup, ~15 minutes)

### Step 1 — Put the site on GitHub

1. Go to [github.com](https://github.com) and sign in (or create a free account).
2. Click the **+** in the top-right corner → **New repository**.
3. Name it something like `kirk-johnson-books`, keep it **Public**, and click **Create repository**.
4. On the new repo page, click **uploading an existing file**.
5. Drag ALL the files and folders from this project into the upload box
   (index.html, about.html, specials.html, contact.html, thanks.html,
   the css folder, and the images folder).
6. Click **Commit changes**.

### Step 2 — Connect Netlify (this is your hosting)

1. Go to [app.netlify.com](https://app.netlify.com) and click **Sign up with GitHub**.
2. Click **Add new site** → **Import an existing project** → **GitHub**.
3. Pick your `kirk-johnson-books` repository.
4. Leave all the build settings blank/default (it's a plain HTML site) and
   click **Deploy site**.
5. In about a minute, your site is live at a netlify.app address. You can
   rename it (Site settings → Change site name) or connect a custom domain
   like kirkjohnsonbooks.com later.

From now on, any time you change a file on GitHub, Netlify automatically
updates the live site within a minute or two.

### Step 3 — Turn on email collection (Netlify Forms)

Both forms (free-chapter signup and contact) are already wired for Netlify.
After your first deploy:

1. In Netlify, open your site and click **Forms** in the left menu.
2. You'll see two forms: **chapter-request** and **contact**.
   Every submission (name, email, which book they want) is saved there.
3. To get an email at kirkinphx@gmail.com every time someone signs up:
   go to **Site settings → Forms → Form notifications → Add notification →
   Email notification**, and enter kirkinphx@gmail.com.

When someone requests a free chapter, you'll get an email with their address
and the book they chose — just reply with the chapter attached. (Netlify's
free plan includes 100 form submissions per month, which is plenty to start.)

## Things you'll want to update

### Replace the Amazon links with your real book pages

Right now each Buy button points to an Amazon **search** for your name and
the title. Once you have the exact Amazon page for each book:

1. Open `index.html`.
2. Find the line for each book that looks like:
   `<a class="btn solid" href="https://www.amazon.com/s?k=River+Boat+Gambler+Kirk+Johnson" ...`
3. Replace the web address in quotes with your book's real Amazon link.

### Write your real bio

Open `about.html` and look for the comment that says **EDIT YOUR BIO HERE**.
Replace those paragraphs with your own story. You can also swap in an author
photo: add it to the `images` folder and change the filename in the
`portrait` section of the same file.

### Editing files after they're on GitHub

You don't need any special software. On GitHub, open any file, click the
pencil icon (Edit), make your change, and click **Commit changes**. Netlify
updates the live site automatically.
