<p align="center"> 
<img style="max-width:100%;" src="https://cdn.svarun.dev/gh/varunsridharan/action-repository-roster/banner.jpg"/>
~ Shout-out supporters in your GitHub README file. ~ 
</p>

## 🚀  Usage
1. [Setup Action Workflow File](#-github-action-workflow-file)
2. Update Your `README.md` with below code

***Repository Stargazers***
```markdown
    ## ↳ Stargazers
    <!-- REPOSITORY_STARS:START --> <!-- REPOSITORY_STARS:END -->
```

***Repository Forks***
```markdown
    ## ↳ Forkers
    <!-- REPOSITORY_FORKS:START --><!-- REPOSITORY_FORKS:END -->
```
> :information_source:  Currently there are ways to auto trigger the workflow when a users **stars** / **forks** the repository.
>
> :information_source:  Using this action with the workflow trigger [fork](https://docs.github.com/en/free-pro-team@latest/actions/reference/events-that-trigger-workflows#fork) & [watch](https://docs.github.com/en/free-pro-team@latest/actions/reference/events-that-trigger-workflows#watch) is the best optmized way.
>
> if you want to remove users that have un-stared / deleted the fork then you might have to use [cron](https://docs.github.com/en/free-pro-team@latest/actions/reference/events-that-trigger-workflows#schedule) to handle it

---

## ⚙️ Configuration
<table>
    <tr>
        <th>Option</th>
        <th>Description</th>
        <th>Default</th>
    </tr>
    <tr> <th colspan="3">General Config</th> </tr>
    <tr>
        <td><code>IMAGE_SAVE_PATH</code></td>
        <td>
            Custom location on where to save generated <strong>SVG</strong> image file. <br/>
            <i>Image Files Are Generated When Output Type Set To <code>image</code></i>
        </td>
        <td><code>.github/roster/</code></td>
    </tr>
    <tr> <th colspan="3">Forks Config</th> </tr>
    <tr>
        <td><code>FORK</code></td>
        <td>
            Set to <strong>true</strong> to generate latest forked users information. or provide a file location to update the information <br/>
            If its set to <strong>FALSE</strong> the forked users information will not be generated
        </td>
        <td><code>README.md</code></td>
    </tr>
    <tr>
        <td><code>FORK_OUTPUT_TYPE</code></td>
        <td>this can be set to either <strong>table</strong>, <strong>list</strong> OR <strong>image</strong></td>
        <td><code>markdown</code></td>
    </tr>
    <tr>
        <td><code>FORK_OUTPUT_STYLE</code></td>
        <td>Please Refer <a href="#paintbrush-styling-options">:paintbrush: Styling Options</a> Below</td>
        <td><code>table</code></td>
    </tr>
    <tr>
        <td><code>FORK_COUNTS</code></td>
        <td>No of latest forked users to generate</td>
        <td><code>7</code></td>
    </tr>
    <tr>
        <td><code>FORK_DESCRIPTION</code></td>
        <td>
            set to <strong>true</strong> to show default description after Forks users information. <br/>
            or you can also provide your custom text to show after the Forks users information.
            if its set to <strong>FALSE</strong> description will not be generated        
        </td>
        <td><code>true</code></td>
    </tr>
    <tr> <th colspan="3">Stars Config</th> </tr>
    <tr>
        <td><code>STARS</code></td>
        <td>
            Set to <strong>true</strong> to generate latest Stargazers users information. or provide a file location to update the information <br/>
            If its set to <strong>FALSE</strong> the Stargazers users information will not be generated
        </td>
        <td><code>README.md</code></td>
    </tr>
    <tr>
        <td><code>STARS_OUTPUT_TYPE</code></td>
        <td>this can be set to either <strong>table</strong>, <strong>list</strong> OR <strong>image</strong></td>
        <td><code>markdown</code></td>
    </tr>
    <tr>
        <td><code>STARS_OUTPUT_STYLE</code></td>
        <td>Please Refer <a href="#paintbrush-styling-options">:paintbrush: Styling Options</a> Below</td>
        <td><code>table</code></td>
    </tr>
    <tr>
        <td><code>STARS_COUNTS</code></td>
        <td>No of latest Stargazers users to generate</td>
        <td><code>7</code></td>
    </tr>
    <tr>
        <td><code>STARS_DESCRIPTION</code></td>
        <td>
            set to <strong>true</strong> to show default description after Stargazers users information. <br/>
            or you can also provide your custom text to show after the Stargazers users information.
            if its set to <strong>FALSE</strong> description will not be generated        
        </td>
        <td><code>true</code></td>
    </tr>
</table>

### :paintbrush: Styling Options
<table>
    <tr>
        <th>Option</th>
        <th>Description</th>
        <th colspan="3">Output Types</th>
    </tr>
    <tr>
        <td colspan="2"></td>
        <th>Image</th>
        <th>Table</th>
        <th>List</th>
    </tr>
    <tr>
        <td><code>no-image</code></td>
        <td>User's avatar will not be rendered</td>
        <td align="center">✔</td>
        <td align="center">✔</td>
        <td align="center">❌</td>
    </tr>
    <tr>
        <td><code>img-smooth</code></td>
        <td>User's avatar will slightly rounded</td>
        <td align="center">✔</td>
        <td align="center">❌</td>
        <td align="center">❌</td>
    </tr>
    <tr>
        <td><code>img-rounded</code></td>
        <td>User's avatar will rounded</td>
        <td align="center">✔</td>
        <td align="center">❌</td>
        <td align="center">❌</td>
    </tr>
    <tr>
        <td><code>img-small</code></td>
        <td>User's avatar will be set to small size</td>
        <td align="center">✔</td>
        <td align="center">✔</td>
        <td align="center">❌</td>
    </tr>
    <tr>
        <td><code>img-large</code></td>
        <td>User's avatar will be set to large size</td>
        <td align="center">✔</td>
        <td align="center">✔</td>
        <td align="center">❌</td>
    </tr>
    <tr>
        <td><code>no-name</code></td>
        <td>User's name will not be rendered</td>
        <td align="center">✔</td>
        <td align="center">✔</td>
        <td align="center">❌</td>
    </tr>
    <tr>
        <td><code>no-link</code></td>
        <td>Link to users github profile will not be added</td>
        <td align="center">❌</td>
        <td align="center">✔</td>
        <td align="center">✔</td>
    </tr>
    <tr>
        <td><code>list-ordered</code></td>
        <td>HTML list will be ordered</td>
        <td align="center">❌</td>
        <td align="center">❌</td>
        <td align="center">✔</td>
    </tr>
    <tr>
        <td><code>bold</code></td>
        <td>username text will be rendered in bold text</td>
        <td align="center">✔</td>
        <td align="center">✔</td>
        <td align="center">✔</td>
    </tr>
    <tr>
        <td><code>italic</code></td>
        <td>username text will be rendered in italic text</td>
        <td align="center">✔</td>
        <td align="center">✔</td>
        <td align="center">✔</td>
    </tr>
    <tr>
        <td><code>small</code></td>
        <td>username text will be rendered in small fontsize text</td>
        <td align="center">✔</td>
        <td align="center">✔</td>
        <td align="center">✔</td>
    </tr>
</table>

> You can provide multiple styles in `*_OUTPUT_STYLE` by entering `,` separated | Example : `img-small,bold,italic`

#### Example Code
 ```yaml
# Below Will Render Stargazers Data In HTML Table With small user avatar
STARS_OUTPUT_TYPE: 'table' # Possible Options [ image , table , list ]
STARS_OUTPUT_STYLE: 'img-small'

# Below Will Render Fork's Data In SVG Image with small user avatar & user's name hidden
FORK_OUTPUT_TYPE: 'image' # Possible Options [ image , table , list ]
FORK_OUTPUT_STYLE: 'img-small,no-name'
 ```

## 🚀 Github Action Workflow File

<!-- START [code:yml|raw] .github/workflows/repo-roster.yml -->
```yml
name: "🙏 Repository Roster"

on:
  workflow_dispatch:
  watch:
    types:
      - started
  fork:

jobs:
  update_latest_roster:
    name: "🐔  Update Latest Roster"
    runs-on: ubuntu-latest
    steps:
      - name: "📥  Fetching Repository Contents"
        uses: actions/checkout@main

      - name: "🐔  Markdown - Repository Roster"
        uses: "varunsridharan/action-repository-roster@main"
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}

```
<!-- END [code:yml|raw] .github/workflows/repo-roster.yml -->


## 🎉 Live Examples (for this repo)

### ↳ Stargazers
<!-- REPOSITORY_STARS:START -->

<!-- REPOSITORY_STARS:END -->

### ↳ Forkers
<!-- REPOSITORY_FORKS:START -->

<!-- REPOSITORY_FORKS:END -->

<p align="center">
    For Styling Demo Please Check <a href="https://github.com/varunsridharan/action-repository-roster/tree/main/examples">Examples Directory</a>
</p>

---

<!-- START common-footer.mustache -->

<!-- END common-footer.mustache -->