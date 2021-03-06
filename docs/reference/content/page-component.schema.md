
# Page Component Schema

```
https://ns.adobe.com/xdm/content/page-component
```

A page component is a part or module of a `Componentized Page` or included in a `Component Container`.
It contains content fragments and has a specific type.
The type determines how the component will be displayed, rendered, and authored.


| [Abstract](../../abstract.md) | [Extensible](../../extensions.md) | [Status](../../status.md) | [Identifiable](../../id.md) | [Custom Properties](../../extensions.md) | [Additional Properties](../../extensions.md) | Defined In |
|-------------------------------|-----------------------------------|---------------------------|-----------------------------|------------------------------------------|----------------------------------------------|------------|
| Can be instantiated | Yes | Experimental | No | Forbidden | Permitted | [content/page-component.schema.json](content/page-component.schema.json) |
## Schema Hierarchy

* Page Component `https://ns.adobe.com/xdm/content/page-component`
  * [Componentized Page](componentized-page.schema.md) `https://ns.adobe.com/xdm/content/componentized-page`


## Page Component Examples

```json
{
  "@type": "https://francois.corp.adobe.com:4502/apps/foundation/image",
  "image": {
    "@type": "https://ns.adobe.com/xdm/assets/asset",
    "repo:id": "urn:aaid:aem:4123ba4c-93a8-4c5d-b979-1234e4318185",
    "@id": "https://francois.corp.adobe.com:4502/content/dam/Glasses-small.jpg"
  }
}
```

```json
{
  "@type": "https://francois.corp.adobe.com:4502/apps/foundation/title",
  "dc:title": "Protect Your Eyes"
}
```


# Page Component Properties

| Property | Type | Required | Defined by |
|----------|------|----------|------------|
| [@type](#@type) | `string` | Optional | Page Component (this schema) |
| `*` | any | Additional | this schema *allows* additional properties |

## @type

Type of the component. Acts as processing hint for the client.

`@type`
* is optional
* type: `string`
* defined in this schema

### @type Type


`string`
* format: `uri` – Uniformous Resource Identifier (according to [RFC3986](http://tools.ietf.org/html/rfc3986))





