# General
## Three ways to process structured data formats.
- **Iteration** - Iterating over Event (or, token) stream.
  + pull parsing
  + push parsing
- **Data Binding** - Binding Json data into Objects (of your favorite language).
- **Tree Traversal** - Building a tree structure (from Json) and traversing it using suitable methods.

# XML
- SAX (iteration, push)
- Streaming API for XML (StAX) (iteration, pull) (JSR-173)
  + https://github.com/FasterXML/woodstox
  + The Sun Java Streaming XML Parser (SJSXP) (part of GlassFish) https://sjsxp.java.net/
- JAXB (data binding)
- DOM, XOM, JDOM, DOM4j (tree traversal)
- XSL Transformations
  + http://www.w3.org/TR/xslt
- XMLBeans
- SOAP

# JSON

## Big JSON files
- https://github.com/zeMirco/sf-city-lots-json

## Libraries
- **http://mvnrepository.com/open-source/json-libraries** - lookup the relevant libraries here.

### Jackson (iteration | data binding | tree traversal)
- https://github.com/FasterXML/jackson
- https://github.com/FasterXML/jackson-databind

### GSON
- https://github.com/google/gson