# Sheltie family tree

An interactive, password-protected family tree for our group of Shetland Sheepdogs.

The page is encrypted with [StatiCrypt](https://github.com/robinmoisson/staticrypt) and hosted on GitHub Pages.

## Never upload the unencrypted file

This repo is public. Only the **encrypted** `index.html` should ever be uploaded here. Keep the unencrypted `sheltie-family-tree.html` on your own computer.

## Updating the page

1. **Get the latest file.** Download the updated `sheltie-family-tree.html`.

2. **Rename it.** Change the name to `index.html`.

3. **Encrypt it.** Open a terminal in the same folder and run:

   ```bash
   npx staticrypt index.html -p "[ADD_PASSWORD]" --template-color-secondary "#F6EFE2" --template-color-primary "#8B5E3C"
   ```

   - Replace `[ADD_PASSWORD]` with the password. Keep the quotes.
   - Node.js must be installed for `npx` to work.
   - The encrypted file is saved as `encrypted/index.html`.
   - Optional: add `--remember 30` so visitors stay logged in for 30 days.

4. **Upload it.** Upload `encrypted/index.html` to this repo, replacing the old `index.html`.

5. **Wait and check.** Wait a minute or two, then refresh the site and log in to check it.

## First-time GitHub Pages setup

Go to **Settings → Pages**. Choose **Deploy from a branch**, then **main** and **/(root)**, and click **Save**.

## Colours used on the login page

- Background: cream `#F6EFE2`
- Button and accent: brown `#8B5E3C`
