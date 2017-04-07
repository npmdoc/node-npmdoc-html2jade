# api documentation for  [html2jade (v0.8.6)](https://github.com/donpark/html2jade#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-html2jade.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-html2jade) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-html2jade.svg)](https://travis-ci.org/npmdoc/node-npmdoc-html2jade)
#### HTML to Jade conversion tool

[![NPM](https://nodei.co/npm/html2jade.png?downloads=true)](https://www.npmjs.com/package/html2jade)

[![apidoc](https://npmdoc.github.io/node-npmdoc-html2jade/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-html2jade_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-html2jade/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-html2jade/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-html2jade/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Don Park",
        "email": "donpark@docuverse.com"
    },
    "bin": {
        "html2jade": "./cli.js"
    },
    "bugs": {
        "url": "https://github.com/donpark/html2jade/issues"
    },
    "dependencies": {
        "commander": "*",
        "he": "^0.4.1",
        "jsdom-little": "^0.10.5"
    },
    "description": "HTML to Jade conversion tool",
    "devDependencies": {
        "async": "*",
        "coffee-script": "~1.6.3",
        "mocha": "*"
    },
    "directories": {},
    "dist": {
        "shasum": "2b3774189d395f77397888e91c8c61ec46e4248b",
        "tarball": "https://registry.npmjs.org/html2jade/-/html2jade-0.8.6.tgz"
    },
    "engines": {
        "node": ">= 0.4.0"
    },
    "gitHead": "29f27cfa901f845360035221778b7aa7876f49b0",
    "homepage": "https://github.com/donpark/html2jade#readme",
    "license": "BSD",
    "main": "./lib/html2jade.js",
    "maintainers": [
        {
            "name": "aichholzer",
            "email": "theaichholzer@gmail.com"
        },
        {
            "name": "donpark",
            "email": "donpark@docuverse.com"
        }
    ],
    "name": "html2jade",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/donpark/html2jade.git"
    },
    "scripts": {
        "prepublish": "coffee -c lib",
        "test": "mocha"
    },
    "version": "0.8.6"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module html2jade](#apidoc.module.html2jade)
1.  [function <span class="apidocSignatureSpan">html2jade.</span>Converter (options)](#apidoc.element.html2jade.Converter)
1.  [function <span class="apidocSignatureSpan">html2jade.</span>Output ()](#apidoc.element.html2jade.Output)
1.  [function <span class="apidocSignatureSpan">html2jade.</span>Parser (options)](#apidoc.element.html2jade.Parser)
1.  [function <span class="apidocSignatureSpan">html2jade.</span>StreamOutput (stream)](#apidoc.element.html2jade.StreamOutput)
1.  [function <span class="apidocSignatureSpan">html2jade.</span>StringOutput ()](#apidoc.element.html2jade.StringOutput)
1.  [function <span class="apidocSignatureSpan">html2jade.</span>Writer (options)](#apidoc.element.html2jade.Writer)
1.  [function <span class="apidocSignatureSpan">html2jade.</span>convert (input, output, options)](#apidoc.element.html2jade.convert)
1.  [function <span class="apidocSignatureSpan">html2jade.</span>convertDocument (document, options, cb)](#apidoc.element.html2jade.convertDocument)
1.  [function <span class="apidocSignatureSpan">html2jade.</span>convertHtml (html, options, cb)](#apidoc.element.html2jade.convertHtml)
1.  object <span class="apidocSignatureSpan">html2jade.</span>Converter.prototype
1.  object <span class="apidocSignatureSpan">html2jade.</span>Output.prototype
1.  object <span class="apidocSignatureSpan">html2jade.</span>Parser.prototype
1.  object <span class="apidocSignatureSpan">html2jade.</span>StreamOutput.prototype
1.  object <span class="apidocSignatureSpan">html2jade.</span>StringOutput.prototype
1.  object <span class="apidocSignatureSpan">html2jade.</span>Writer.prototype

#### [module html2jade.Converter](#apidoc.module.html2jade.Converter)
1.  [function <span class="apidocSignatureSpan">html2jade.</span>Converter (options)](#apidoc.element.html2jade.Converter.Converter)

#### [module html2jade.Converter.prototype](#apidoc.module.html2jade.Converter.prototype)
1.  [function <span class="apidocSignatureSpan">html2jade.Converter.prototype.</span>children (parent, output, indent)](#apidoc.element.html2jade.Converter.prototype.children)
1.  [function <span class="apidocSignatureSpan">html2jade.Converter.prototype.</span>comment (node, output)](#apidoc.element.html2jade.Converter.prototype.comment)
1.  [function <span class="apidocSignatureSpan">html2jade.Converter.prototype.</span>conditional (node, condition, output)](#apidoc.element.html2jade.Converter.prototype.conditional)
1.  [function <span class="apidocSignatureSpan">html2jade.Converter.prototype.</span>document (document, output)](#apidoc.element.html2jade.Converter.prototype.document)
1.  [function <span class="apidocSignatureSpan">html2jade.Converter.prototype.</span>element (node, output)](#apidoc.element.html2jade.Converter.prototype.element)
1.  [function <span class="apidocSignatureSpan">html2jade.Converter.prototype.</span>script (node, output, tagHead, tagAttr)](#apidoc.element.html2jade.Converter.prototype.script)
1.  [function <span class="apidocSignatureSpan">html2jade.Converter.prototype.</span>style (node, output, tagHead, tagAttr)](#apidoc.element.html2jade.Converter.prototype.style)
1.  [function <span class="apidocSignatureSpan">html2jade.Converter.prototype.</span>text (node, output, options)](#apidoc.element.html2jade.Converter.prototype.text)

#### [module html2jade.Output](#apidoc.module.html2jade.Output)
1.  [function <span class="apidocSignatureSpan">html2jade.</span>Output ()](#apidoc.element.html2jade.Output.Output)

#### [module html2jade.Output.prototype](#apidoc.module.html2jade.Output.prototype)
1.  [function <span class="apidocSignatureSpan">html2jade.Output.prototype.</span>enter ()](#apidoc.element.html2jade.Output.prototype.enter)
1.  [function <span class="apidocSignatureSpan">html2jade.Output.prototype.</span>leave ()](#apidoc.element.html2jade.Output.prototype.leave)
1.  [function <span class="apidocSignatureSpan">html2jade.Output.prototype.</span>write (data, indent)](#apidoc.element.html2jade.Output.prototype.write)
1.  [function <span class="apidocSignatureSpan">html2jade.Output.prototype.</span>writeln (data, indent)](#apidoc.element.html2jade.Output.prototype.writeln)

#### [module html2jade.Parser](#apidoc.module.html2jade.Parser)
1.  [function <span class="apidocSignatureSpan">html2jade.</span>Parser (options)](#apidoc.element.html2jade.Parser.Parser)

#### [module html2jade.Parser.prototype](#apidoc.module.html2jade.Parser.prototype)
1.  [function <span class="apidocSignatureSpan">html2jade.Parser.prototype.</span>parse (arg, cb)](#apidoc.element.html2jade.Parser.prototype.parse)

#### [module html2jade.StreamOutput](#apidoc.module.html2jade.StreamOutput)
1.  [function <span class="apidocSignatureSpan">html2jade.</span>StreamOutput (stream)](#apidoc.element.html2jade.StreamOutput.StreamOutput)
1.  object <span class="apidocSignatureSpan">html2jade.StreamOutput.</span>__super__

#### [module html2jade.StreamOutput.prototype](#apidoc.module.html2jade.StreamOutput.prototype)
1.  [function <span class="apidocSignatureSpan">html2jade.StreamOutput.prototype.</span>constructor (stream)](#apidoc.element.html2jade.StreamOutput.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">html2jade.StreamOutput.prototype.</span>write (data, indent)](#apidoc.element.html2jade.StreamOutput.prototype.write)
1.  [function <span class="apidocSignatureSpan">html2jade.StreamOutput.prototype.</span>writeln (data, indent)](#apidoc.element.html2jade.StreamOutput.prototype.writeln)

#### [module html2jade.StringOutput](#apidoc.module.html2jade.StringOutput)
1.  [function <span class="apidocSignatureSpan">html2jade.</span>StringOutput ()](#apidoc.element.html2jade.StringOutput.StringOutput)
1.  object <span class="apidocSignatureSpan">html2jade.StringOutput.</span>__super__

#### [module html2jade.StringOutput.prototype](#apidoc.module.html2jade.StringOutput.prototype)
1.  [function <span class="apidocSignatureSpan">html2jade.StringOutput.prototype.</span>constructor ()](#apidoc.element.html2jade.StringOutput.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">html2jade.StringOutput.prototype.</span>final ()](#apidoc.element.html2jade.StringOutput.prototype.final)
1.  [function <span class="apidocSignatureSpan">html2jade.StringOutput.prototype.</span>write (data, indent)](#apidoc.element.html2jade.StringOutput.prototype.write)
1.  [function <span class="apidocSignatureSpan">html2jade.StringOutput.prototype.</span>writeln (data, indent)](#apidoc.element.html2jade.StringOutput.prototype.writeln)

#### [module html2jade.Writer](#apidoc.module.html2jade.Writer)
1.  [function <span class="apidocSignatureSpan">html2jade.</span>Writer (options)](#apidoc.element.html2jade.Writer.Writer)

#### [module html2jade.Writer.prototype](#apidoc.module.html2jade.Writer.prototype)
1.  [function <span class="apidocSignatureSpan">html2jade.Writer.prototype.</span>breakLine (line)](#apidoc.element.html2jade.Writer.prototype.breakLine)
1.  [function <span class="apidocSignatureSpan">html2jade.Writer.prototype.</span>buildTagAttr (attrName, attrValue)](#apidoc.element.html2jade.Writer.prototype.buildTagAttr)
1.  [function <span class="apidocSignatureSpan">html2jade.Writer.prototype.</span>forEachChild (parent, cb)](#apidoc.element.html2jade.Writer.prototype.forEachChild)
1.  [function <span class="apidocSignatureSpan">html2jade.Writer.prototype.</span>tagAttr (node, indents)](#apidoc.element.html2jade.Writer.prototype.tagAttr)
1.  [function <span class="apidocSignatureSpan">html2jade.Writer.prototype.</span>tagHead (node)](#apidoc.element.html2jade.Writer.prototype.tagHead)
1.  [function <span class="apidocSignatureSpan">html2jade.Writer.prototype.</span>tagText (node)](#apidoc.element.html2jade.Writer.prototype.tagText)
1.  [function <span class="apidocSignatureSpan">html2jade.Writer.prototype.</span>writeText (node, output, options)](#apidoc.element.html2jade.Writer.prototype.writeText)
1.  [function <span class="apidocSignatureSpan">html2jade.Writer.prototype.</span>writeTextContent (node, output, options)](#apidoc.element.html2jade.Writer.prototype.writeTextContent)
1.  [function <span class="apidocSignatureSpan">html2jade.Writer.prototype.</span>writeTextLine (node, line, output, options)](#apidoc.element.html2jade.Writer.prototype.writeTextLine)



# <a name="apidoc.module.html2jade"></a>[module html2jade](#apidoc.module.html2jade)

#### <a name="apidoc.element.html2jade.Converter"></a>[function <span class="apidocSignatureSpan">html2jade.</span>Converter (options)](#apidoc.element.html2jade.Converter)
- description and source-code
```javascript
function Converter(options) {
  var _ref, _ref1;
  this.options = options != null ? options : {};
  this.scalate = (_ref = this.options.scalate) != null ? _ref : false;
  this.writer = (_ref1 = this.options.writer) != null ? _ref1 : new Writer(this.options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.html2jade.Output"></a>[function <span class="apidocSignatureSpan">html2jade.</span>Output ()](#apidoc.element.html2jade.Output)
- description and source-code
```javascript
function Output() {
  this.indents = '';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.html2jade.Parser"></a>[function <span class="apidocSignatureSpan">html2jade.</span>Parser (options)](#apidoc.element.html2jade.Parser)
- description and source-code
```javascript
function Parser(options) {
  this.options = options != null ? options : {};
  if (isNode) {
    this.jsdom = require('jsdom-little');
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.html2jade.StreamOutput"></a>[function <span class="apidocSignatureSpan">html2jade.</span>StreamOutput (stream)](#apidoc.element.html2jade.StreamOutput)
- description and source-code
```javascript
function StreamOutput(stream) {
  this.stream = stream;
  StreamOutput.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.html2jade.StringOutput"></a>[function <span class="apidocSignatureSpan">html2jade.</span>StringOutput ()](#apidoc.element.html2jade.StringOutput)
- description and source-code
```javascript
function StringOutput() {
  StringOutput.__super__.constructor.apply(this, arguments);
  this.fragments = [];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.html2jade.Writer"></a>[function <span class="apidocSignatureSpan">html2jade.</span>Writer (options)](#apidoc.element.html2jade.Writer)
- description and source-code
```javascript
function Writer(options) {
  var _ref, _ref1, _ref2;
  if (options == null) {
    options = {};
  }
  this.wrapLength = (_ref = options.wrapLength) != null ? _ref : 80;
  this.scalate = (_ref1 = options.scalate) != null ? _ref1 : false;
  this.attrSep = this.scalate || options.noattrcomma ? ' ' : ', ';
  if (options.double) {
    this.attrQuote = '"';
    this.nonAttrQuote = "'";
  } else {
    this.attrQuote = "'";
    this.nonAttrQuote = '"';
  }
  this.attrQuoteEscaped = "\\" + this.attrQuote;
  this.noEmptyPipe = (_ref2 = options.noemptypipe) != null ? _ref2 : false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.html2jade.convert"></a>[function <span class="apidocSignatureSpan">html2jade.</span>convert (input, output, options)](#apidoc.element.html2jade.convert)
- description and source-code
```javascript
convert = function (input, output, options) {
  if (options == null) {
    options = {};
  }
  applyOptions(options);
  if (options.parser == null) {
    options.parser = new Parser(options);
  }
  return options.parser.parse(input, function(errors, window) {
    if (errors != null ? errors.length : void 0) {
      return errors;
    } else {
      if (output == null) {
        output = new StreamOutput(process.stdout);
      }
      if (options.converter == null) {
        options.converter = new Converter(options);
      }
      return options.converter.document(window.document, output);
    }
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.html2jade.convertDocument"></a>[function <span class="apidocSignatureSpan">html2jade.</span>convertDocument (document, options, cb)](#apidoc.element.html2jade.convertDocument)
- description and source-code
```javascript
convertDocument = function (document, options, cb) {
  var output, _ref;
  if (options == null) {
    options = {};
  }
  applyOptions(options);
  output = (_ref = options.output) != null ? _ref : new StringOutput();
  if (options.converter == null) {
    options.converter = new Converter(options);
  }
  options.converter.document(document, output);
  if (cb != null) {
    return cb(null, output.final());
  }
}
```
- example usage
```shell
...
    html2jade.convertHtml(html, {}, function (err, jade) {
      // do your thing
    });

To convert DOM document into Jade (client-side):

    // assumes html2jade.js file has been loaded
    Html2Jade.convertDocument(document, {}, function (err, jade) {
      // do your thing
    });

## Converting Mustache/Handlebars Templates

Jade is commonly used to generate HTML with embedded Mustache or Handlebars templates.
...
```

#### <a name="apidoc.element.html2jade.convertHtml"></a>[function <span class="apidocSignatureSpan">html2jade.</span>convertHtml (html, options, cb)](#apidoc.element.html2jade.convertHtml)
- description and source-code
```javascript
convertHtml = function (html, options, cb) {
  if (options == null) {
    options = {};
  }
  applyOptions(options);
  if (options.parser == null) {
    options.parser = new Parser(options);
  }
  return options.parser.parse(html, function(errors, window) {
    var output, _ref;
    if (errors != null ? errors.length : void 0) {
      return errors;
    } else {
      output = (_ref = options.output) != null ? _ref : new StringOutput();
      if (options.converter == null) {
        options.converter = new Converter(options);
      }
      options.converter.document(window.document, output);
      if (cb != null) {
        return cb(null, output.final());
      }
    }
  });
}
```
- example usage
```shell
...

## Programmatic Usage (>= 0.0.7)

To convert raw HTML into Jade:

var html2jade = require('html2jade');
var html = "<html><body>Hello World</body></html>";
html2jade.convertHtml(html, {}, function (err, jade) {
  // do your thing
});

To convert DOM document into Jade (client-side):

// assumes html2jade.js file has been loaded
Html2Jade.convertDocument(document, {}, function (err, jade) {
...
```



# <a name="apidoc.module.html2jade.Converter"></a>[module html2jade.Converter](#apidoc.module.html2jade.Converter)

#### <a name="apidoc.element.html2jade.Converter.Converter"></a>[function <span class="apidocSignatureSpan">html2jade.</span>Converter (options)](#apidoc.element.html2jade.Converter.Converter)
- description and source-code
```javascript
function Converter(options) {
  var _ref, _ref1;
  this.options = options != null ? options : {};
  this.scalate = (_ref = this.options.scalate) != null ? _ref : false;
  this.writer = (_ref1 = this.options.writer) != null ? _ref1 : new Writer(this.options);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.html2jade.Converter.prototype"></a>[module html2jade.Converter.prototype](#apidoc.module.html2jade.Converter.prototype)

#### <a name="apidoc.element.html2jade.Converter.prototype.children"></a>[function <span class="apidocSignatureSpan">html2jade.Converter.prototype.</span>children (parent, output, indent)](#apidoc.element.html2jade.Converter.prototype.children)
- description and source-code
```javascript
children = function (parent, output, indent) {
  var _this = this;
  if (indent == null) {
    indent = true;
  }
  if (indent) {
    output.enter();
  }
  this.writer.forEachChild(parent, function(child) {
    var nodeType;
    nodeType = child.nodeType;
    if (nodeType === 1) {
      return _this.element(child, output);
    } else if (nodeType === 3) {
      if (parent._nodeName === 'code') {
        return _this.text(child, output, {
          encodeEntityRef: true,
          pipe: true
        });
      } else {
        return _this.text(child, output, doNotEncode ? {
          encodeEntityRef: false
        } : {
          encodeEntityRef: true
        });
      }
    } else if (nodeType === 8) {
      return _this.comment(child, output);
    }
  });
  if (indent) {
    return output.leave();
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.html2jade.Converter.prototype.comment"></a>[function <span class="apidocSignatureSpan">html2jade.Converter.prototype.</span>comment (node, output)](#apidoc.element.html2jade.Converter.prototype.comment)
- description and source-code
```javascript
comment = function (node, output) {
  var condition, data, lines,
    _this = this;
  condition = node.data.match(/\s*\[(if\s+[^\]]+)\]/);
  if (!condition) {
    data = node.data || '';
    if (data.length === 0 || data.search(/\r|\n/) === -1) {
      return output.writeln("// " + (data.trim()));
    } else {
      output.writeln('//');
      output.enter();
      lines = data.split(/\r|\n/);
      lines.forEach(function(line) {
        return _this.writer.writeTextLine(node, line, output, {
          pipe: false,
          trim: true,
          wrap: false
        });
      });
      return output.leave();
    }
  } else {
    return this.conditional(node, condition[1], output);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.html2jade.Converter.prototype.conditional"></a>[function <span class="apidocSignatureSpan">html2jade.Converter.prototype.</span>conditional (node, condition, output)](#apidoc.element.html2jade.Converter.prototype.conditional)
- description and source-code
```javascript
conditional = function (node, condition, output) {
  var conditionalElem, innerHTML;
  innerHTML = node.textContent.trim().replace(/\s*\[if\s+[^\]]+\]>\s*/, '').replace('<![endif]', '');
  if (innerHTML.indexOf("<!") === 0) {
    condition = " [" + condition + "] <!";
    innerHTML = null;
  }
  conditionalElem = node.ownerDocument.createElement('conditional');
  conditionalElem.setAttribute('condition', condition);
  if (innerHTML) {
    conditionalElem.innerHTML = innerHTML;
  }
  return node.parentNode.insertBefore(conditionalElem, node.nextSibling);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.html2jade.Converter.prototype.document"></a>[function <span class="apidocSignatureSpan">html2jade.Converter.prototype.</span>document (document, output)](#apidoc.element.html2jade.Converter.prototype.document)
- description and source-code
```javascript
document = function (document, output) {
  var docTypeName, doctype, htmlEls, publicId, systemId;
  if (document.doctype != null) {
    doctype = document.doctype;
    docTypeName = void 0;
    publicId = doctype.publicId;
    systemId = doctype.systemId;
    if ((publicId != null) && (publicIdDocTypeNames[publicId] != null)) {
      docTypeName = publicIdDocTypeNames[publicId];
    } else if ((systemId != null) && (systemIdDocTypeNames[systemId] != null)) {
      docTypeName = systemIdDocTypeNames[systemId] != null;
    } else if ((doctype.name != null) && doctype.name.toLowerCase() === 'html') {
      docTypeName = 'html';
    }
    if (docTypeName != null) {
      output.writeln('doctype ' + docTypeName);
    }
  }
  if (document.documentElement) {
    return this.children(document, output, false);
  } else {
    htmlEls = document.getElementsByTagName('html');
    if (htmlEls.length > 0) {
      return this.element(htmlEls[0], output);
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.html2jade.Converter.prototype.element"></a>[function <span class="apidocSignatureSpan">html2jade.Converter.prototype.</span>element (node, output)](#apidoc.element.html2jade.Converter.prototype.element)
- description and source-code
```javascript
element = function (node, output) {
  var firstline, tagAttr, tagHead, tagName, tagText,
    _this = this;
  if (!(node != null ? node.tagName : void 0)) {
    return;
  }
  tagName = node.tagName.toLowerCase();
  tagHead = this.writer.tagHead(node);
  tagAttr = this.writer.tagAttr(node, output.indents);
  tagText = this.writer.tagText(node);
  if (tagName === 'script' || tagName === 'style') {
    if (node.hasAttribute('src')) {
      output.writeln(tagHead + tagAttr);
      return this.writer.writeTextContent(node, output, {
        pipe: false,
        wrap: false
      });
    } else if (tagName === 'script') {
      return this.script(node, output, tagHead, tagAttr);
    } else if (tagName === 'style') {
      return this.style(node, output, tagHead, tagAttr);
    }
  } else if (tagName === 'conditional') {
    output.writeln('//' + node.getAttribute('condition'));
    return this.children(node, output);
  } else if (['pre'].indexOf(tagName) !== -1) {
    output.writeln(tagHead + tagAttr + '.');
    output.enter();
    firstline = true;
    this.writer.forEachChild(node, function(child) {
      var data;
      if (child.nodeType === 3) {
        data = child.data;
        if ((data != null) && data.length > 0) {
          if (firstline) {
            if (data.search(/\r\n|\r|\n/) === 0) {
              data = data.replace(/\r\n|\r|\n/, '');
            }
            data = '\\n' + data;
            firstline = false;
          }
          data = data.replace(/\t/g, '\\t');
          data = data.replace(/\r\n|\r|\n/g, '\n' + output.indents);
          return output.write(data);
        }
      }
    });
    output.writeln();
    return output.leave();
  } else if (this.options.bodyless && (tagName === 'html' || tagName === 'body')) {
    return this.children(node, output, false);
  } else if (tagText) {
    if (doNotEncode) {
      return output.writeln(tagHead + tagAttr + ' ' + tagText);
    } else {
      return output.writeln(tagHead + tagAttr + ' ' + Ent.encode(tagText, entOptions));
    }
  } else {
    output.writeln(tagHead + tagAttr);
    return this.children(node, output);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.html2jade.Converter.prototype.script"></a>[function <span class="apidocSignatureSpan">html2jade.Converter.prototype.</span>script (node, output, tagHead, tagAttr)](#apidoc.element.html2jade.Converter.prototype.script)
- description and source-code
```javascript
script = function (node, output, tagHead, tagAttr) {
  if (this.scalate) {
    output.writeln(':javascript');
    return this.writer.writeTextContent(node, output, {
      pipe: false,
      wrap: false
    });
  } else {
    output.writeln("" + tagHead + tagAttr + ".");
    return this.writer.writeTextContent(node, output, {
      pipe: false,
      trim: true,
      wrap: false,
      escapeBackslash: true
    });
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.html2jade.Converter.prototype.style"></a>[function <span class="apidocSignatureSpan">html2jade.Converter.prototype.</span>style (node, output, tagHead, tagAttr)](#apidoc.element.html2jade.Converter.prototype.style)
- description and source-code
```javascript
style = function (node, output, tagHead, tagAttr) {
  if (this.scalate) {
    output.writeln(':css');
    return this.writer.writeTextContent(node, output, {
      pipe: false,
      wrap: false
    });
  } else {
    output.writeln("" + tagHead + tagAttr + ".");
    return this.writer.writeTextContent(node, output, {
      pipe: false,
      trim: true,
      wrap: false
    });
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.html2jade.Converter.prototype.text"></a>[function <span class="apidocSignatureSpan">html2jade.Converter.prototype.</span>text (node, output, options)](#apidoc.element.html2jade.Converter.prototype.text)
- description and source-code
```javascript
text = function (node, output, options) {
  node.normalize();
  return this.writer.writeText(node, output, options);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.html2jade.Output"></a>[module html2jade.Output](#apidoc.module.html2jade.Output)

#### <a name="apidoc.element.html2jade.Output.Output"></a>[function <span class="apidocSignatureSpan">html2jade.</span>Output ()](#apidoc.element.html2jade.Output.Output)
- description and source-code
```javascript
function Output() {
  this.indents = '';
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.html2jade.Output.prototype"></a>[module html2jade.Output.prototype](#apidoc.module.html2jade.Output.prototype)

#### <a name="apidoc.element.html2jade.Output.prototype.enter"></a>[function <span class="apidocSignatureSpan">html2jade.Output.prototype.</span>enter ()](#apidoc.element.html2jade.Output.prototype.enter)
- description and source-code
```javascript
enter = function () {
  var i, _i, _results;
  if (useTabs) {
    return this.indents += '\t';
  } else {
    _results = [];
    for (i = _i = 1; 1 <= nspaces ? _i <= nspaces : _i >= nspaces; i = 1 <= nspaces ? ++_i : --_i) {
      _results.push(this.indents += ' ');
    }
    return _results;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.html2jade.Output.prototype.leave"></a>[function <span class="apidocSignatureSpan">html2jade.Output.prototype.</span>leave ()](#apidoc.element.html2jade.Output.prototype.leave)
- description and source-code
```javascript
leave = function () {
  if (useTabs) {
    return this.indents = this.indents.substring(1);
  } else {
    return this.indents = this.indents.substring(nspaces);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.html2jade.Output.prototype.write"></a>[function <span class="apidocSignatureSpan">html2jade.Output.prototype.</span>write (data, indent)](#apidoc.element.html2jade.Output.prototype.write)
- description and source-code
```javascript
write = function (data, indent) {
  if (indent == null) {
    indent = true;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.html2jade.Output.prototype.writeln"></a>[function <span class="apidocSignatureSpan">html2jade.Output.prototype.</span>writeln (data, indent)](#apidoc.element.html2jade.Output.prototype.writeln)
- description and source-code
```javascript
writeln = function (data, indent) {
  if (indent == null) {
    indent = true;
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.html2jade.Parser"></a>[module html2jade.Parser](#apidoc.module.html2jade.Parser)

#### <a name="apidoc.element.html2jade.Parser.Parser"></a>[function <span class="apidocSignatureSpan">html2jade.</span>Parser (options)](#apidoc.element.html2jade.Parser.Parser)
- description and source-code
```javascript
function Parser(options) {
  this.options = options != null ? options : {};
  if (isNode) {
    this.jsdom = require('jsdom-little');
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.html2jade.Parser.prototype"></a>[module html2jade.Parser.prototype](#apidoc.module.html2jade.Parser.prototype)

#### <a name="apidoc.element.html2jade.Parser.prototype.parse"></a>[function <span class="apidocSignatureSpan">html2jade.Parser.prototype.</span>parse (arg, cb)](#apidoc.element.html2jade.Parser.prototype.parse)
- description and source-code
```javascript
parse = function (arg, cb) {
  var parser, window;
  if (!arg) {
    return cb('null file');
  } else {
    if (this.options.inputType === "file") {
      arg = FS.readFileSync(arg, "utf8");
    }
    if (isNode) {
      return this.jsdom.env(arg, cb);
    } else {
      window = {};
      parser = new DOMParser();
      window.document = parser.parseFromString(arg, "text/html");
      return cb(null, window);
    }
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.html2jade.StreamOutput"></a>[module html2jade.StreamOutput](#apidoc.module.html2jade.StreamOutput)

#### <a name="apidoc.element.html2jade.StreamOutput.StreamOutput"></a>[function <span class="apidocSignatureSpan">html2jade.</span>StreamOutput (stream)](#apidoc.element.html2jade.StreamOutput.StreamOutput)
- description and source-code
```javascript
function StreamOutput(stream) {
  this.stream = stream;
  StreamOutput.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.html2jade.StreamOutput.prototype"></a>[module html2jade.StreamOutput.prototype](#apidoc.module.html2jade.StreamOutput.prototype)

#### <a name="apidoc.element.html2jade.StreamOutput.prototype.constructor"></a>[function <span class="apidocSignatureSpan">html2jade.StreamOutput.prototype.</span>constructor (stream)](#apidoc.element.html2jade.StreamOutput.prototype.constructor)
- description and source-code
```javascript
function StreamOutput(stream) {
  this.stream = stream;
  StreamOutput.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.html2jade.StreamOutput.prototype.write"></a>[function <span class="apidocSignatureSpan">html2jade.StreamOutput.prototype.</span>write (data, indent)](#apidoc.element.html2jade.StreamOutput.prototype.write)
- description and source-code
```javascript
write = function (data, indent) {
  if (indent == null) {
    indent = true;
  }
  if (data == null) {
    data = '';
  }
  if (indent) {
    return this.stream.write(this.indents + data);
  } else {
    return this.stream.write(data);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.html2jade.StreamOutput.prototype.writeln"></a>[function <span class="apidocSignatureSpan">html2jade.StreamOutput.prototype.</span>writeln (data, indent)](#apidoc.element.html2jade.StreamOutput.prototype.writeln)
- description and source-code
```javascript
writeln = function (data, indent) {
  if (indent == null) {
    indent = true;
  }
  if (data == null) {
    data = '';
  }
  if (indent) {
    return this.stream.write(this.indents + data + '\n');
  } else {
    return this.stream.write(data + '\n');
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.html2jade.StringOutput"></a>[module html2jade.StringOutput](#apidoc.module.html2jade.StringOutput)

#### <a name="apidoc.element.html2jade.StringOutput.StringOutput"></a>[function <span class="apidocSignatureSpan">html2jade.</span>StringOutput ()](#apidoc.element.html2jade.StringOutput.StringOutput)
- description and source-code
```javascript
function StringOutput() {
  StringOutput.__super__.constructor.apply(this, arguments);
  this.fragments = [];
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.html2jade.StringOutput.prototype"></a>[module html2jade.StringOutput.prototype](#apidoc.module.html2jade.StringOutput.prototype)

#### <a name="apidoc.element.html2jade.StringOutput.prototype.constructor"></a>[function <span class="apidocSignatureSpan">html2jade.StringOutput.prototype.</span>constructor ()](#apidoc.element.html2jade.StringOutput.prototype.constructor)
- description and source-code
```javascript
function StringOutput() {
  StringOutput.__super__.constructor.apply(this, arguments);
  this.fragments = [];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.html2jade.StringOutput.prototype.final"></a>[function <span class="apidocSignatureSpan">html2jade.StringOutput.prototype.</span>final ()](#apidoc.element.html2jade.StringOutput.prototype.final)
- description and source-code
```javascript
final = function () {
  var result;
  result = this.fragments.join('');
  this.fragments = [];
  return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.html2jade.StringOutput.prototype.write"></a>[function <span class="apidocSignatureSpan">html2jade.StringOutput.prototype.</span>write (data, indent)](#apidoc.element.html2jade.StringOutput.prototype.write)
- description and source-code
```javascript
write = function (data, indent) {
  if (indent == null) {
    indent = true;
  }
  if (data == null) {
    data = '';
  }
  if (indent) {
    return this.fragments.push(this.indents + data);
  } else {
    return this.fragments.push(data);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.html2jade.StringOutput.prototype.writeln"></a>[function <span class="apidocSignatureSpan">html2jade.StringOutput.prototype.</span>writeln (data, indent)](#apidoc.element.html2jade.StringOutput.prototype.writeln)
- description and source-code
```javascript
writeln = function (data, indent) {
  if (indent == null) {
    indent = true;
  }
  if (data == null) {
    data = '';
  }
  if (indent) {
    return this.fragments.push(this.indents + data + '\n');
  } else {
    return this.fragments.push(data + '\n');
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.html2jade.Writer"></a>[module html2jade.Writer](#apidoc.module.html2jade.Writer)

#### <a name="apidoc.element.html2jade.Writer.Writer"></a>[function <span class="apidocSignatureSpan">html2jade.</span>Writer (options)](#apidoc.element.html2jade.Writer.Writer)
- description and source-code
```javascript
function Writer(options) {
  var _ref, _ref1, _ref2;
  if (options == null) {
    options = {};
  }
  this.wrapLength = (_ref = options.wrapLength) != null ? _ref : 80;
  this.scalate = (_ref1 = options.scalate) != null ? _ref1 : false;
  this.attrSep = this.scalate || options.noattrcomma ? ' ' : ', ';
  if (options.double) {
    this.attrQuote = '"';
    this.nonAttrQuote = "'";
  } else {
    this.attrQuote = "'";
    this.nonAttrQuote = '"';
  }
  this.attrQuoteEscaped = "\\" + this.attrQuote;
  this.noEmptyPipe = (_ref2 = options.noemptypipe) != null ? _ref2 : false;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.html2jade.Writer.prototype"></a>[module html2jade.Writer.prototype](#apidoc.module.html2jade.Writer.prototype)

#### <a name="apidoc.element.html2jade.Writer.prototype.breakLine"></a>[function <span class="apidocSignatureSpan">html2jade.Writer.prototype.</span>breakLine (line)](#apidoc.element.html2jade.Writer.prototype.breakLine)
- description and source-code
```javascript
breakLine = function (line) {
  var lines, word, words;
  if (!line || line.length === 0) {
    return [];
  }
  if (line.search(/\s+/ === -1)) {
    return [line];
  }
  lines = [];
  words = line.split(/\s+/);
  line = '';
  while (words.length) {
    word = words.shift();
    if (line.length + word.length > this.wrapLength) {
      lines.push(line);
      line = word;
    } else if (line.length) {
      line += ' ' + word;
    } else {
      line = word;
    }
  }
  if (line.length) {
    lines.push(line);
  }
  return lines;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.html2jade.Writer.prototype.buildTagAttr"></a>[function <span class="apidocSignatureSpan">html2jade.Writer.prototype.</span>buildTagAttr (attrName, attrValue)](#apidoc.element.html2jade.Writer.prototype.buildTagAttr)
- description and source-code
```javascript
buildTagAttr = function (attrName, attrValue) {
  if (attrValue.indexOf(this.attrQuote) === -1) {
    return attrName + "=" + this.attrQuote + attrValue + this.attrQuote;
  } else if (attrValue.indexOf(this.nonAttrQuote) === -1) {
    return attrName + "=" + this.nonAttrQuote + attrValue + this.nonAttrQuote;
  } else {
    attrValue = attrValue.replace(new RegExp(this.attrQuote, 'g'), this.attrQuoteEscaped);
    return attrName + "=" + this.attrQuote + attrValue + this.attrQuote;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.html2jade.Writer.prototype.forEachChild"></a>[function <span class="apidocSignatureSpan">html2jade.Writer.prototype.</span>forEachChild (parent, cb)](#apidoc.element.html2jade.Writer.prototype.forEachChild)
- description and source-code
```javascript
forEachChild = function (parent, cb) {
  var child, _results;
  if (parent) {
    child = parent.firstChild;
    _results = [];
    while (child) {
      cb(child);
      _results.push(child = child.nextSibling);
    }
    return _results;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.html2jade.Writer.prototype.tagAttr"></a>[function <span class="apidocSignatureSpan">html2jade.Writer.prototype.</span>tagAttr (node, indents)](#apidoc.element.html2jade.Writer.prototype.tagAttr)
- description and source-code
```javascript
tagAttr = function (node, indents) {
  var attr, attrName, attrValue, attrs, invalidClassNames, result, _i, _len;
  if (indents == null) {
    indents = '';
  }
  attrs = node.attributes;
  if (!attrs || attrs.length === 0) {
    return '';
  } else {
    result = [];
    for (_i = 0, _len = attrs.length; _i < _len; _i++) {
      attr = attrs[_i];
      if (attr && attr.nodeName) {
        attrName = attr.nodeName;
        attrValue = attr.nodeValue;
        if (attrName === 'id' && isValidJadeId(attrValue)) {

        } else if (attrName === 'class') {
          invalidClassNames = node.getAttribute('class').split(/\s+/).filter(function(item) {
            return item && !isValidJadeClassName(item);
          });
          if (invalidClassNames.length > 0) {
            result.push(this.buildTagAttr(attrName, invalidClassNames.join(' ')));
          }
        } else {
          attrValue = attrValue.replace(/(\r|\n)\s*/g, "\\$1" + indents);
          result.push(this.buildTagAttr(attrName, attrValue));
        }
      }
    }
    if (result.length > 0) {
      return "(" + (result.join(this.attrSep)) + ")";
    } else {
      return '';
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.html2jade.Writer.prototype.tagHead"></a>[function <span class="apidocSignatureSpan">html2jade.Writer.prototype.</span>tagHead (node)](#apidoc.element.html2jade.Writer.prototype.tagHead)
- description and source-code
```javascript
tagHead = function (node) {
  var result, validClassNames;
  result = node.tagName !== 'DIV' ? node.tagName.toLowerCase() : '';
  if (node.id && isValidJadeId(node.id)) {
    result += "#" + node.id;
  }
  if (node.hasAttribute('class') && node.getAttribute('class').length > 0) {
    validClassNames = node.getAttribute('class').split(/\s+/).filter(function(item) {
      return item && isValidJadeClassName(item);
    });
    result += '.' + validClassNames.join('.');
  }
  if (result.length === 0) {
    result = 'div';
  }
  return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.html2jade.Writer.prototype.tagText"></a>[function <span class="apidocSignatureSpan">html2jade.Writer.prototype.</span>tagText (node)](#apidoc.element.html2jade.Writer.prototype.tagText)
- description and source-code
```javascript
tagText = function (node) {
  var data, _ref;
  if (((_ref = node.firstChild) != null ? _ref.nodeType : void 0) !== 3) {
    return null;
  } else if (node.firstChild !== node.lastChild) {
    return null;
  } else {
    data = node.firstChild.data;
    if (data.length > this.wrapLength || data.match(/\r|\n/)) {
      return null;
    } else {
      return data;
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.html2jade.Writer.prototype.writeText"></a>[function <span class="apidocSignatureSpan">html2jade.Writer.prototype.</span>writeText (node, output, options)](#apidoc.element.html2jade.Writer.prototype.writeText)
- description and source-code
```javascript
writeText = function (node, output, options) {
  var data, lines,
    _this = this;
  if (node.nodeType === 3) {
    data = node.data || '';
    if (data.length > 0) {
      lines = data.split(/\r|\n/);
      return lines.forEach(function(line) {
        return _this.writeTextLine(node, line, output, options);
      });
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.html2jade.Writer.prototype.writeTextContent"></a>[function <span class="apidocSignatureSpan">html2jade.Writer.prototype.</span>writeTextContent (node, output, options)](#apidoc.element.html2jade.Writer.prototype.writeTextContent)
- description and source-code
```javascript
writeTextContent = function (node, output, options) {
  var _this = this;
  output.enter();
  this.forEachChild(node, function(child) {
    return _this.writeText(child, output, options);
  });
  return output.leave();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.html2jade.Writer.prototype.writeTextLine"></a>[function <span class="apidocSignatureSpan">html2jade.Writer.prototype.</span>writeTextLine (node, line, output, options)](#apidoc.element.html2jade.Writer.prototype.writeTextLine)
- description and source-code
```javascript
writeTextLine = function (node, line, output, options) {
  var encodeEntityRef, escapeBackslash, lines, pipe, prefix, trim, wrap, _ref, _ref1, _ref2, _ref3, _ref4, _ref5, _ref6,
    _this = this;
  if (options == null) {
    options = {};
  }
  pipe = (_ref = options.pipe) != null ? _ref : true;
  trim = (_ref1 = options.trim) != null ? _ref1 : false;
  wrap = (_ref2 = options.wrap) != null ? _ref2 : true;
  encodeEntityRef = (_ref3 = options.encodeEntityRef) != null ? _ref3 : false;
  escapeBackslash = (_ref4 = options.escapeBackslash) != null ? _ref4 : false;
  if (pipe && this.noEmptyPipe && line.trim().length === 0) {
    return;
  }
  prefix = pipe ? '| ' : '';
  if ((node != null ? (_ref5 = node.previousSibling) != null ? _ref5.nodeType : void 0 : void 0) !== 1) {
    line = line.trimLeft();
  }
  if ((node != null ? (_ref6 = node.nextSibling) != null ? _ref6.nodeType : void 0 : void 0) !== 1) {
    line = line.trimRight();
  }
  if (line) {
    if (encodeEntityRef) {
      line = Ent.encode(line, entOptions);
    }
    if (escapeBackslash) {
      line = line.replace("\\", "\\\\");
    }
    if (!wrap || line.length <= this.wrapLength) {
      return output.writeln(prefix + line);
    } else {
      lines = this.breakLine(line);
      if (lines.length === 1) {
        return output.writeln(prefix + line);
      } else {
        return lines.forEach(function(line) {
          return _this.writeTextLine(node, line, output, options);
        });
      }
    }
  }
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
