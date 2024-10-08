<div align="center">

<h2>xorshift32</h2>

[![JSR](https://jsr.io/badges/@studiowebux/xorshift32)](https://jsr.io/@studiowebux/xorshift32)

<p>Typescript implementation of xorshift32.</p>

<p align="center">
  <a href="https://github.com/studiowebux/xorshift32/issues">Report Bug</a>
  ·
  <a href="https://github.com/studiowebux/xorshift32/issues">Request Feature</a>
</p>
</div>

---

## Installation and Usage

1. Install deno: https://deno.com
2. `deno add @studiowebux/xorshift32`


```ts
const prng = initialize_prng(123456);

const integer = generate_integer(prng);
const min_max_interger = generate_min_max_integer(prng, 1, 3); // min is inclusive and max is exclusive
const float = generate_float(prng);

const saved_state = save_prng_state(prng);
load_prng_state(prng, saved_state);
```


### Releases and Github Actions

```bash
git tag -a X.Y.Z -m "Version X.Y.Z"
git push origin tags/X.Y.Z
```

---

## Contributing

1. Fork the project
2. Create a Feature Branch
3. Commit your changes
4. Push your changes
5. Create a PR

<details>
<summary>Working with your local branch</summary>

**Branch Checkout:**

```bash
git checkout -b <feature|fix|release|chore|hotfix>/prefix-name
```

> Your branch name must starts with [feature|fix|release|chore|hotfix] and use a / before the name;
> Use hyphens as separator;
> The prefix correspond to your Kanban tool id (e.g. abc-123)

**Keep your branch synced:**

```bash
git fetch origin
git rebase origin/master
```

**Commit your changes:**

```bash
git add .
git commit -m "<feat|ci|test|docs|build|chore|style|refactor|perf|BREAKING CHANGE>: commit message"
```

> Follow this convention commitlint for your commit message structure

**Push your changes:**

```bash
git push origin <feature|fix|release|chore|hotfix>/prefix-name
```

**Examples:**

```bash
git checkout -b release/v1.15.5
git checkout -b feature/abc-123-something-awesome
git checkout -b hotfix/abc-432-something-bad-to-fix
```

```bash
git commit -m "docs: added awesome documentation"
git commit -m "feat: added new feature"
git commit -m "test: added tests"
```

</details>

## License

Distributed under the MIT License. See LICENSE for more information.

## Contact

- Tommy Gingras @ tommy@studiowebux.com | Studio Webux

<div>
<b> | </b>
<a href="https://www.buymeacoffee.com/studiowebux" target="_blank"
      ><img
        src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png"
        alt="Buy Me A Coffee"
        style="height: 30px !important; width: 105px !important"
        height="30"
        width="105"
/></a>
<b> | </b>
<a href="https://webuxlab.com" target="_blank"
      ><img
        src="https://webuxlab-static.s3.ca-central-1.amazonaws.com/logoAmpoule.svg"
        alt="Webux Logo"
        style="height: 30px !important"
        height="30"
/> Webux Lab</a>
<b> | </b>
</div>
