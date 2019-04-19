# Sass files for TUJ website
It includes Core 4.0 and Core 4.1 files, as well as section specific files. Core 4.0 (core.scss) is used on all the pages except the UG section. Core 4.1 (core-4.1.scss) is used for the UG section.

## Updating and maintaining the Sass files
When updating the Sass files, work on the Sass files from this repo.

- Make sure this repo is up-to-date.
- Make sure you pull the files before you update your local files.

1. git pull
2. Update .scss and generate .css.
3. Upload only .css files to the TEST/LIVE sites.
4. git push when you are done.

## Component Library
Component library for Core 4.0 can be found at the following URL:

- https://www.tuj.ac.jp/style-guide/
- https://www.tuj.ac.jp/jp/style-guide/

## How Styles Are Organized
### Core
Core has the styles for all basic elements used on the TUJ website. Core 4.0 is used for all sections except the undergraduate section. Core 4.1 is used for UG section only.

### Section Specific Styles
Section specific styles, such as UG only styles, are written in section specific styles sheet, such as ug.scss.  If there are multiple pages that use the same style in a particular section, add them to the section specific style sheet.

#### Main section
```html
<link rel="stylesheet" href="/css/core.css?v=201902181557" />
```

#### UG section
```html
<link rel="stylesheet" href="/css/core-4.1.css" />
<link rel="stylesheet" href="/css/ug.css" />
```

#### TESOL section
```html
<link rel="stylesheet" href="/css/core.css?v=201902181557" />
<link rel="stylesheet" href="/css/tesol.css" />
```

### Page Specific Styles
If the styles are only used on a particular page, put it on the document itself.  It might be best to use SSI to include the css instead of loading an external CSS for this.

## Grid System
See sample grid below:

- https://www.tuj.ac.jp/style-guide/grid.html
