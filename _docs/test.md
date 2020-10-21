---
permalink: /test/
name: Test
---

## Buttons

Make any link standout more when applying the `.btn .btn--primary` classes.

```html
<a href="#" class="btn btn--primary">Link Text</a>
```

| Button Type   | Example                                   | Class                      | Kramdown                                    |
| ------------- | ----------------------------------------- | -------------------------- | ------------------------------------------- |
| Default       | [Text](#link){: .btn}                     | `.btn`                     | `[Text](#link){: .btn}`                     |
| Primary       | [Text](#link){: .btn .btn--primary}       | `.btn .btn--primary`       | `[Text](#link){: .btn .btn--primary}`       |
| Success       | [Text](#link){: .btn .btn--success}       | `.btn .btn--success`       | `[Text](#link){: .btn .btn--success}`       |
| Warning       | [Text](#link){: .btn .btn--warning}       | `.btn .btn--warning`       | `[Text](#link){: .btn .btn--warning}`       |
| Danger        | [Text](#link){: .btn .btn--danger}        | `.btn .btn--danger`        | `[Text](#link){: .btn .btn--danger}`        |
| Info          | [Text](#link){: .btn .btn--info}          | `.btn .btn--info`          | `[Text](#link){: .btn .btn--info}`          |
| Inverse       | [Text](#link){: .btn .btn--inverse}       | `.btn .btn--inverse`       | `[Text](#link){: .btn .btn--inverse}`       |
| Light Outline | [Text](#link){: .btn .btn--light-outline} | `.btn .btn--light-outline` | `[Text](#link){: .btn .btn--light-outline}` |

| Button Size | Example                                                 | Class                              | Kramdown                                            |
| ----------- | ------------------------------------------------------- | ---------------------------------- | --------------------------------------------------- |
| X-Large     | [X-Large Button](#){: .btn .btn--primary .btn--x-large} | `.btn .btn--primary .btn--x-large` | `[Text](#link){: .btn .btn--primary .btn--x-large}` |
| Large       | [Large Button](#){: .btn .btn--primary .btn--large}     | `.btn .btn--primary .btn--large`   | `[Text](#link){: .btn .btn--primary .btn--large}`   |
| Default     | [Default Button](#){: .btn .btn--primary}               | `.btn .btn--primary`               | `[Text](#link){: .btn .btn--primary }`              |
| Small       | [Small Button](#){: .btn .btn--primary .btn--small}     | `.btn .btn--primary .btn--small`   | `[Text](#link){: .btn .btn--primary .btn--small}`   |

## Notices

Call attention to a block of text.

| Notice Type | Class              |
| ----------- | ------------------ |
| Default     | `.notice`          |
| Primary     | `.notice--primary` |
| Info        | `.notice--info`    |
| Warning     | `.notice--warning` |
| Success     | `.notice--success` |
| Danger      | `.notice--danger`  |

**Watch out!** This paragraph of text has been [emphasized](#) with the `{: .notice}` class.
{: .notice}

**Watch out!** This paragraph of text has been [emphasized](#) with the `{: .notice--primary}` class.
{: .notice--primary}

**Watch out!** This paragraph of text has been [emphasized](#) with the `{: .notice--info}` class.
{: .notice--info}

**Watch out!** This paragraph of text has been [emphasized](#) with the `{: .notice--warning}` class.
{: .notice--warning}

**Watch out!** This paragraph of text has been [emphasized](#) with the `{: .notice--success}` class.
{: .notice--success}

**Watch out!** This paragraph of text has been [emphasized](#) with the `{: .notice--danger}` class.
{: .notice--danger}

{% capture notice-text %}
You can also add the `.notice` class to a `<div>` element.

* Bullet point 1
* Bullet point 2
{% endcapture %}

<div class="notice--info">
  <h4 class="no_toc">Notice Headline:</h4>
  {{ notice-text | markdownify }}
</div>
