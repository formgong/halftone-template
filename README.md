# Halftone — architecture studio site with a Formgong form

**Live demo:** https://halftone.formgong.com · Download: the [latest release](https://github.com/formgong/halftone-template/releases/latest) zip.

[![Deploy to Cloudflare](https://deploy.workers.cloudflare.com/button)](https://deploy.workers.cloudflare.com/?url=https://github.com/formgong/halftone-template) [![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https%3A%2F%2Fgithub.com%2Fformgong%2Fhalftone-template&project-name=halftone&repository-name=halftone)

Each button copies the site to your GitHub and publishes it. Then replace `fk_your_access_key` in `index.html` of your copy with your Formgong access key (free at https://formgong.com/new) and commit: the host republishes on its own.

Шаблон сайту архітектурного бюро з формою Формгонг

A standalone one-page template for an architecture or design studio, in a single `index.html`. The demo studio, TAKU in Copenhagen, and its projects are fictional.

- **Loader.** An orange screen with four corner words and the page itself, tilted and small, in the middle. When the count reaches 100 it straightens and fills the screen.
- **Header.** Three blocks in a row, inset from the edges: Menu, the mark and Get in touch. It hides on the way down and comes back on the way up.
- **Hero.** A pinned photo behind a fine halftone dot screen, with the title split to the two edges. As you scroll, the photo turns into a second frame.
- **Projects.** Full-screen photos that stack as you scroll, each with a white bar along the bottom.
- **The big words.** Huge words; a strip of photos rises over them and the middle photo opens to the whole screen, then a text panel slides in.
- **Services and numbers.** A services list, and numbers on orange that count up beside a pattern of rounded tiles.
- **Footer.** A footer with the big wordmark.
- **Contact.** An orange contact card over a photo, with Instagram, Email and LinkedIn along the bottom.

## English

**Set up the form**

1. Create a form in the Formgong dashboard and copy its access key.
2. In `index.html`, replace `fk_your_access_key` with that key.
3. Optional: put your Turnstile site key in `data-sitekey` on `<form id="fg-form">`.

The form sends `name`, `email` and `message`. It shows "thank you" only when the server answers `success: true`, and shows the error otherwise.

**Edit**

- Colours are `--accent` and `--accent-2` (the hero title gradient) at the top of the styles.
- Sizes follow `--u`, one 1920th of the window, so the page scales as one drawing. Below 760px it switches to a phone layout.
- With `prefers-reduced-motion: reduce` there is no loader, the scroll effects are off and every section shows its final state.

**Images.** All ten were made for this template with FLUX.1 [schnell] (Apache 2.0) on the free AI Horde. You may use them in your own site. Replace them with photos of your own work, keeping the file names.

## Українська

Окремий шаблон для архітектурного або дизайн-бюро в одному `index.html`. На сторінці по черзі:

- помаранчевий лоадер з нахиленою мініатюрою сторінки;
- шапка з трьох блоків;
- головне фото під растровими крапками із заголовком, розведеним до країв;
- проєкти на весь екран, що наїжджають один на одного;
- величезні слова, на які піднімається смуга фото;
- блок із цифрами на помаранчевому тлі;
- великий логотип у підвалі;
- форма в помаранчевій картці.

**Форма:** замініть `fk_your_access_key` на ключ форми з кабінету Формгонг. Форма надсилає ім'я, пошту й повідомлення.

**Картинки:** усі згенеровано для цього шаблону моделлю FLUX.1 [schnell] (ліцензія Apache 2.0) через безкоштовний AI Horde. Замініть їх фото своїх робіт, зберігши назви файлів.
