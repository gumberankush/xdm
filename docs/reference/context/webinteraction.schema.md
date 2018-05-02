
# Web Interaction Schema

```
https://ns.adobe.com/xdm/context/webinteraction
```

The Web Interaction schema captures information about interactions that happened on a web page after the intial page load (see also Web Page View) was completed.

It is intended for recording interactions in rich web applications that do not trigger a new page load such as single page web apps (SPAs).


| Abstract | Extensible | Status | Identifiable | Custom Properties | Additional Properties | Defined In |
|----------|------------|--------|--------------|-------------------|-----------------------|------------|
| Can be instantiated | Yes | Experimental | No | Forbidden | Permitted | [context/webinteraction.schema.json](context/webinteraction.schema.json) |

## Web Interaction Example
```json
{
  "xdm:type": "other",
  "xdm:URL": "https://www.example.com/products/store/?view=1",
  "xdm:name": "product store"
}
```

# Web Interaction Properties

| Property | Type | Required | Defined by |
|----------|------|----------|------------|
| [xdm:URL](#xdmurl) | `string` | Optional | Web Interaction (this schema) |
| [xdm:name](#xdmname) | `string` | Optional | Web Interaction (this schema) |
| [xdm:type](#xdmtype) | `enum` | Optional | Web Interaction (this schema) |
| `*` | any | Additional | this schema *allows* additional properties |

## xdm:URL
### URL

The actual link/URL used for this web interaction

`xdm:URL`
* is optional
* type: `string`
* defined in this schema

### xdm:URL Type


`string`






## xdm:name
### Name

The normative name used for this web link, used for classification purposes

`xdm:name`
* is optional
* type: `string`
* defined in this schema

### xdm:name Type


`string`






## xdm:type
### Type

The link type.

`xdm:type`
* is optional
* type: `enum`
* defined in this schema

The value of this property **must** be equal to one of the [known values below](#xdm:type-known-values).

### xdm:type Known Values
| Value | Description |
|-------|-------------|
| `download` | Download |
| `exit` | Exit |
| `other` | Other |


