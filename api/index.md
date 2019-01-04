# API Docs

<a href="{{ site.baseurl }}"><- Go back to main page/site.</a>

## **GET** Tools and Dictionary


[`{{ site.url }}{{ site.baseurl }}/api/v1/tools_and_dictionary.json`](/v1/tools_and_dictionary.json)

Returns all open government policy tools and data portals and Data Dictionary.

**Return type:** Object / dict of dictionary and data.
```js
{
  "data-dictionary": {...},
  "data": [{...}, ...]
}
```

## **GET** Dictionary


[`{{ site.url }}{{site.baseurl }}/api/v1/dictionary.json`](/v1/dictionary.json)

Returns data dictionary of tools object / dict.

**Return type:** Object / dict.
```js
{
  "Jurisdiction": "Definition...",
  "Level of Government": "",
  "Policy Name": "",
  "Policy Tool": "",
  "Policy Adopted": "",
  "Portal/Catalogue Launched": "",
  "Portal/Catalogue Platform": "",
  "Content Type": "",
  "License": ""
}
```

## **GET** Tools


[`{{ site.url }}{{ site.baseurl }}/api/v1/tools.json`](/v1/tools.json)

Returns all open government policy tools and data portals.

**Return type:** Array / List of objects/dicts.
```js
[
  {
    "Jurisdiction": "",
    "Level of Government": "",
    "Policy Name": "",
    "Policy Tool": "",
    "Policy Adopted": "",
    "Portal/Catalogue Launched": "",
    "Portal/Catalogue Platform": "",
    "Content Type": "",
    "License": ""
  },
  {...},
  ...
]
```

