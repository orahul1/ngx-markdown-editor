# ngx-markdown-editor
Angular markdown editor based on ace editor

[![peerDependencies Status](https://david-dm.org/lon-yang/ngx-markdown-editor/peer-status.svg)](https://david-dm.org/lon-yang/ngx-markdown-editor?type=peer)
[![npm version](https://badge.fury.io/js/ngx-markdown-editor.svg)](https://badge.fury.io/js/ngx-markdown-editor)
[![licence](https://img.shields.io/npm/l/ngx-markdown-editor.svg)](https://opensource.org/licenses/Apache2.0)

# Usage

- Add `Ace`、`marked`、`highlight` and `fortawesome` lib

```html
<link href="https://cdn.bootcss.com/font-awesome/4.7.0/css/font-awesome.min.css" rel="stylesheet">
<link href="https://cdn.bootcss.com/highlight.js/9.12.0/styles/agate.min.css" rel="stylesheet">
<script src="https://cdn.bootcss.com/ace/1.2.8/ace.js"></script>
<script src="https://cdn.bootcss.com/marked/0.3.6/marked.min.js"></script>
<script src="https://cdn.bootcss.com/highlight.js/9.12.0/highlight.min.js"></script>
```

- Install `ngx-markdown-editor`

```bash
npm i ngx-markdown-editor
```

- Use markdown-editor component

```ts
import { LMarkdownEditorModule } from 'ngx-markdown-editor';

@NgModule({
  declarations: [
    AppComponent
  ],
  imports: [
    BrowserModule,
    FormsModule,
    LMarkdownEditorModule
  ],
  providers: [],
  bootstrap: [AppComponent]
})
export class AppModule { }
```
```html
<md-editor name="Content" [(ngModel)]="content" [height]="'200px'" required maxlength="500"></md-editor>
```

# Options
- ngModel: markdown original content
- height: editor height
- hideToolbar: hide toolbar, default is false
- required: for form validate
- maxlength: for form validate
