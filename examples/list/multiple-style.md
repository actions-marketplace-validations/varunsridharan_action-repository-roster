# bold,italic,list-ordered
Username will be bold & italic & Users list will be generated using HTML `ol` _Ordered list_

### ↳ Stargazers

<!-- REPOSITORY_STARS:START -->
<ol><li><a href="https://github.com/dexit" rel="nofollow"><b><i>@dexit</i></b> <br/> </a> </li><li><a href="https://github.com/trinitybranding" rel="nofollow"><b><i>@trinitybranding</i></b> <br/> </a> </li></ol><p align="center"><i><b>2</b> have starred this repository</i></p>
<!-- REPOSITORY_STARS:END -->

### ↳ Forkers

<!-- REPOSITORY_FORKS:START -->
<ol><li><a href="https://github.com/dexit" rel="nofollow"><b><i>@dexit</i></b> <br/> </a> </li><li><a href="https://github.com/trinitybranding" rel="nofollow"><b><i>@trinitybranding</i></b> <br/> </a> </li></ol><p align="center"><i><b>2</b> have forked this repository</i></p>
<!-- REPOSITORY_FORKS:END -->

---

```yml
- name: "🐔  Update Repository Roster"
  uses: "varunsridharan/action-repository-roster@main"
  with:
    STARS_OUTPUT_TYPE: "list"
    FORK_OUTPUT_TYPE: "list"
    STARS_OUTPUT_STYLE: "bold,italic,list-ordered"
    FORK_OUTPUT_STYLE: "bold,italic,list-ordered"
  env:
    GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
```