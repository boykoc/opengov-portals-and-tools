# Open Government Portals and Policy Tools Across Canada

This is an adaptation of a chart found on page 23 of the OpenNorth _[What Could Open Data Programs Gain from Aligning with International Best Practices?](http://public.citizenbudget.com/uploads/custom/on.ca/ODCinCanada.pdf)_ report from 2016.

This chart summarizes open government portals and policy tools in Canada at a Federal, Provincial and Municipal level.

We hope to use this webpage as an ongoing record of the current Open Government portal and policy tool landscape across Canada and would love as many updates and additions as possible.

## Contributing

You can use the [editor on GitHub](https://github.com/boykoc/opengov-portals-and-tools/edit/master/README.md) to make updates to the content for this site. Once you save the changes, submit a Pull Request (PR) to request the update.

You can also [email](mailto:opengov@ontario.ca) us or create an [issue on Github](https://github.com/boykoc/opengov-portals-and-tools/issues) if you have changes you'd like to see but aren't familiaur with Pull Requests.

Whenever a something new is committed to the Master branch of this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages of the site, based on the content in the Markdown files.

This site is built with Github Pages, Jekyll and is styled in Markdown (for more details on Markdown see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/)).

## Charts

__These charts scroll left to right to view all columns. New columns may be added.__

### Federal

<table>
  <thead>
    <tr>
      <th>Jurisdiction</th>
      <th>Policy Name</th>
      <th>Policy Tool</th>
      <th>Policy Adopted</th>
      <th>Portal/Catalogue Launched</th>
      <th>Portal/Catalogue Platform</th>
      <th>Content Type</th>
      <th>License</th>
    </tr>
  </thead>
  <tbody>
    {% assign tools = site.data.tools.data | where: "Level of Government", "Federal" %}
    {% for tool in tools %}
      <tr>
        <td>{{ tool.Jurisdiction }}</td>
        <td>{{ tool["Policy Name"] }}</td>
        <td>{{ tool["Policy Tool"] }}</td>
        <td>{{ tool["Policy Adopted"] }}</td>
        <td>{{ tool["Portal/Catalogue Launched"] }}</td>
        <td>{{ tool["Portal/Catalogue Platform"] }}</td>
        <td>{{ tool["Content Type"] }}</td>
        <td>{{ tool["License"] }}</td>
      </tr>
    {% endfor %}
  </tbody>
</table>

### Provincial

<table>
  <thead>
    <tr>
      <th>Jurisdiction</th>
      <th>Policy Name</th>
      <th>Policy Tool</th>
      <th>Policy Adopted</th>
      <th>Portal/Catalogue Launched</th>
      <th>Portal/Catalogue Platform</th>
      <th>Content Type</th>
      <th>License</th>
    </tr>
  </thead>
  <tbody>
    {% assign tools = site.data.tools.data | where: "Level of Government", "Provincial" %}
    {% for tool in tools %}
      <tr>
        <td>{{ tool.Jurisdiction }}</td>
        <td>{{ tool["Policy Name"] }}</td>
        <td>{{ tool["Policy Tool"] }}</td>
        <td>{{ tool["Policy Adopted"] }}</td>
        <td>{{ tool["Portal/Catalogue Launched"] }}</td>
        <td>{{ tool["Portal/Catalogue Platform"] }}</td>
        <td>{{ tool["Content Type"] }}</td>
        <td>{{ tool["License"] }}</td>
      </tr>
    {% endfor %}
  </tbody>
</table>

### Municipal

<table>
  <thead>
    <tr>
      <th>Jurisdiction</th>
      <th>Policy Name</th>
      <th>Policy Tool</th>
      <th>Policy Adopted</th>
      <th>Portal/Catalogue Launched</th>
      <th>Portal/Catalogue Platform</th>
      <th>Content Type</th>
      <th>License</th>
    </tr>
  </thead>
  <tbody>
    {% assign tools = site.data.tools.data | where: "Level of Government", "Municipal" %}
    {% for tool in tools %}
      <tr>
        <td>{{ tool.Jurisdiction }}</td>
        <td>{{ tool["Policy Name"] }}</td>
        <td>{{ tool["Policy Tool"] }}</td>
        <td>{{ tool["Policy Adopted"] }}</td>
        <td>{{ tool["Portal/Catalogue Launched"] }}</td>
        <td>{{ tool["Portal/Catalogue Platform"] }}</td>
        <td>{{ tool["Content Type"] }}</td>
        <td>{{ tool["License"] }}</td>
      </tr>
    {% endfor %}
  </tbody>
</table>

### Data Dictionary

{% assign dictionary = site.data.tools.data-dictionary %}
<dl>
  {% for item in dictionary %}
    <dt>{{ item[0] }}</dt>
    <dd>{{ item[1] }}</dd>
  {% endfor %}
</dl>
