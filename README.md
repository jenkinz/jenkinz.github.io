# jenkinz.github.io

This is my personal résumé site. It's generated using
[JSON Resume](https://jsonresume.org/) with a custom theme modifed from the
default [jsonresume-theme-flat](https://github.com/erming/jsonresume-theme-flat).

## Development Setup

1. Install

        npm install

2. Serve locally

        resume serve --theme jsonresume-theme-bjenkins

3. Export for GitHub Pages deployment

        resume export index.html --format html --theme jsonresume-theme-bjenkins

4. Export a PDF version

        resume export brianjenkins_resume.pdf --format pdf --theme ./jsonresume-theme-bjenkins/

4. Patch `index.html` to add PDF download link

        <section class="row">
            <aside class="col-sm-3"></aside>
            <div class="col-sm-9">
                <a href="/brianjenkins_resume.pdf">Download PDF</a>
            </div>
        </section>

Note: if any changes are made to the theme in `./jsonresume-theme-bjenkins`, you
must reinstall the theme using `npm install ./jsonresume-theme-bjenkins` so the
changes are deployed.

Note: the helper script, `generate.sh`, will run steps 3 and 4 above.
