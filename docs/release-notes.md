# Release Notes

## Latest Changes

### Internal

* ⬆ Bump pillow from 11.1.0 to 11.2.1. PR [#1198](https://github.com/fastapi/typer/pull/1198) by [@dependabot[bot]](https://github.com/apps/dependabot).
* ⬆ Bump cairosvg from 2.7.1 to 2.8.2. PR [#1226](https://github.com/fastapi/typer/pull/1226) by [@dependabot[bot]](https://github.com/apps/dependabot).
* ⬆ Bump ruff from 0.11.6 to 0.11.13. PR [#1241](https://github.com/fastapi/typer/pull/1241) by [@dependabot[bot]](https://github.com/apps/dependabot).

## 0.16.0

### Upgrades

* ⬆️ Add compatibility with Click 8.2. PR [#1222](https://github.com/fastapi/typer/pull/1222) by [@tiangolo](https://github.com/tiangolo).

When using the `CliRunner` with Click < 8.2, to be able to access the `stderr` output, you needed to set the `mix_stderr` parameter to `True`. Since Click 8.2 (and Typer 0.160 this release supporting it) this is no longer necessary, so this parameter has been removed.

### Refactors

* ✅ Refactor tests for compatibility with Click 8.2. PR [#1230](https://github.com/fastapi/typer/pull/1230) by [@tiangolo](https://github.com/tiangolo).

### Internal

* 🔧 Remove Google Analytics. PR [#1229](https://github.com/fastapi/typer/pull/1229) by [@tiangolo](https://github.com/tiangolo).

## 0.15.4

### Upgrades

* 📌 Pin Click to < 8.2, compatibility for Click >= 8.2 will be added in a future version. PR [#1225](https://github.com/fastapi/typer/pull/1225) by [@tiangolo](https://github.com/tiangolo).

## 0.15.3

### Fixes

* 🐛 Ensure that autocompletion works for `Path` arguments/options. PR [#1138](https://github.com/fastapi/typer/pull/1138) by [@svlandeg](https://github.com/svlandeg).
* 🐛 Fix newline after header in help text, and add more tests for the behaviour of `rich_markup_mode` . PR [#964](https://github.com/fastapi/typer/pull/964) by [@svlandeg](https://github.com/svlandeg).

### Internal

* ⬆ Bump astral-sh/setup-uv from 5 to 6. PR [#1203](https://github.com/fastapi/typer/pull/1203) by [@dependabot[bot]](https://github.com/apps/dependabot).
* ⬆ Bump ruff from 0.11.2 to 0.11.6. PR [#1200](https://github.com/fastapi/typer/pull/1200) by [@dependabot[bot]](https://github.com/apps/dependabot).
* ⬆ [pre-commit.ci] pre-commit autoupdate. PR [#1196](https://github.com/fastapi/typer/pull/1196) by [@pre-commit-ci[bot]](https://github.com/apps/pre-commit-ci).
* ⬆ Bump ruff from 0.11.1 to 0.11.2. PR [#1186](https://github.com/fastapi/typer/pull/1186) by [@dependabot[bot]](https://github.com/apps/dependabot).
* ⬆ [pre-commit.ci] pre-commit autoupdate. PR [#1187](https://github.com/fastapi/typer/pull/1187) by [@pre-commit-ci[bot]](https://github.com/apps/pre-commit-ci).
* ⬆ Bump ruff from 0.11.0 to 0.11.1. PR [#1185](https://github.com/fastapi/typer/pull/1185) by [@dependabot[bot]](https://github.com/apps/dependabot).
* ⬆ Bump ruff from 0.9.10 to 0.11.0. PR [#1180](https://github.com/fastapi/typer/pull/1180) by [@dependabot[bot]](https://github.com/apps/dependabot).
* ⬆ [pre-commit.ci] pre-commit autoupdate. PR [#1181](https://github.com/fastapi/typer/pull/1181) by [@pre-commit-ci[bot]](https://github.com/apps/pre-commit-ci).
* ⬆ [pre-commit.ci] pre-commit autoupdate. PR [#1176](https://github.com/fastapi/typer/pull/1176) by [@pre-commit-ci[bot]](https://github.com/apps/pre-commit-ci).
* ⬆ Bump ruff from 0.9.9 to 0.9.10. PR [#1175](https://github.com/fastapi/typer/pull/1175) by [@dependabot[bot]](https://github.com/apps/dependabot).
* ⬆ [pre-commit.ci] pre-commit autoupdate. PR [#1171](https://github.com/fastapi/typer/pull/1171) by [@pre-commit-ci[bot]](https://github.com/apps/pre-commit-ci).
* ⬆ Bump ruff from 0.9.7 to 0.9.9. PR [#1166](https://github.com/fastapi/typer/pull/1166) by [@dependabot[bot]](https://github.com/apps/dependabot).
* ✏️ Fix typo in test name. PR [#1165](https://github.com/fastapi/typer/pull/1165) by [@svlandeg](https://github.com/svlandeg).

## 0.15.2

### Features

* ✨ Allow custom styles for commands in help output. PR [#1103](https://github.com/fastapi/typer/pull/1103) by [@TheTechromancer](https://github.com/TheTechromancer).
* ✨ Avoid the unnecessary import of `typing_extensions` in newer Python versions. PR [#1048](https://github.com/fastapi/typer/pull/1048) by [@horta](https://github.com/horta).

### Fixes

* 🐛 Fix shell completions for the fish shell. PR [#1069](https://github.com/fastapi/typer/pull/1069) by [@goraje](https://github.com/goraje).

### Refactors

* 🚚 Rename test to corner-cases to make it more explicit. PR [#1083](https://github.com/fastapi/typer/pull/1083) by [@tiangolo](https://github.com/tiangolo).

### Docs

* ✏️ Fix small typos in the tutorial documentation. PR [#1137](https://github.com/fastapi/typer/pull/1137) by [@svlandeg](https://github.com/svlandeg).
* 📝 Update optional CLI argument section in tutorial with `Annotated`. PR [#983](https://github.com/fastapi/typer/pull/983) by [@gkeuccsr](https://github.com/gkeuccsr).
* 📝 Clarify the need for `mix_stderr` when accessing the output of `stderr` in tests. PR [#1045](https://github.com/fastapi/typer/pull/1045) by [@mrchrisadams](https://github.com/mrchrisadams).

### Internal

* 🔧 Add support for Python 3.13, tests in CI and add PyPI trove classifier. PR [#1091](https://github.com/fastapi/typer/pull/1091) by [@edgarrmondragon](https://github.com/edgarrmondragon).
* ⬆ Bump ruff from 0.9.6 to 0.9.7. PR [#1161](https://github.com/fastapi/typer/pull/1161) by [@dependabot[bot]](https://github.com/apps/dependabot).
* ⬆ [pre-commit.ci] pre-commit autoupdate. PR [#1162](https://github.com/fastapi/typer/pull/1162) by [@pre-commit-ci[bot]](https://github.com/apps/pre-commit-ci).
* ⬆ Bump ruff from 0.9.5 to 0.9.6. PR [#1153](https://github.com/fastapi/typer/pull/1153) by [@dependabot[bot]](https://github.com/apps/dependabot).
* ⬆ [pre-commit.ci] pre-commit autoupdate. PR [#1151](https://github.com/fastapi/typer/pull/1151) by [@pre-commit-ci[bot]](https://github.com/apps/pre-commit-ci).
* ⬆ Bump ruff from 0.9.4 to 0.9.5. PR [#1146](https://github.com/fastapi/typer/pull/1146) by [@dependabot[bot]](https://github.com/apps/dependabot).
* ⬆ [pre-commit.ci] pre-commit autoupdate. PR [#1142](https://github.com/fastapi/typer/pull/1142) by [@pre-commit-ci[bot]](https://github.com/apps/pre-commit-ci).
* ⬆ Bump ruff from 0.9.3 to 0.9.4. PR [#1139](https://github.com/fastapi/typer/pull/1139) by [@dependabot[bot]](https://github.com/apps/dependabot).
* ⬆ [pre-commit.ci] pre-commit autoupdate. PR [#1135](https://github.com/fastapi/typer/pull/1135) by [@pre-commit-ci[bot]](https://github.com/apps/pre-commit-ci).
* ⬆ Bump ruff from 0.9.1 to 0.9.3. PR [#1136](https://github.com/fastapi/typer/pull/1136) by [@dependabot[bot]](https://github.com/apps/dependabot).
* ⬆ [pre-commit.ci] pre-commit autoupdate. PR [#1130](https://github.com/fastapi/typer/pull/1130) by [@pre-commit-ci[bot]](https://github.com/apps/pre-commit-ci).
* ⬆ Bump ruff from 0.8.6 to 0.9.1. PR [#1118](https://github.com/fastapi/typer/pull/1118) by [@dependabot[bot]](https://github.com/apps/dependabot).
* ⬆ Bump pypa/gh-action-pypi-publish from 1.12.3 to 1.12.4. PR [#1132](https://github.com/fastapi/typer/pull/1132) by [@dependabot[bot]](https://github.com/apps/dependabot).
* ⬆ Bump mkdocs-material from 9.5.49 to 9.5.50. PR [#1129](https://github.com/fastapi/typer/pull/1129) by [@dependabot[bot]](https://github.com/apps/dependabot).
* 💚 Fix test matrix for Python 3.7. PR [#1116](https://github.com/fastapi/typer/pull/1116) by [@svlandeg](https://github.com/svlandeg).
* ⬆ Bump ruff from 0.8.4 to 0.8.6. PR [#1107](https://github.com/fastapi/typer/pull/1107) by [@dependabot[bot]](https://github.com/apps/dependabot).
* ⬆ [pre-commit.ci] pre-commit autoupdate. PR [#1109](https://github.com/fastapi/typer/pull/1109) by [@pre-commit-ci[bot]](https://github.com/apps/pre-commit-ci).
* ⬆ Bump pillow from 11.0.0 to 11.1.0. PR [#1104](https://github.com/fastapi/typer/pull/1104) by [@dependabot[bot]](https://github.com/apps/dependabot).
* ⬆ [pre-commit.ci] pre-commit autoupdate. PR [#1102](https://github.com/fastapi/typer/pull/1102) by [@pre-commit-ci[bot]](https://github.com/apps/pre-commit-ci).
* ⬆ Bump ruff from 0.8.3 to 0.8.4. PR [#1097](https://github.com/fastapi/typer/pull/1097) by [@dependabot[bot]](https://github.com/apps/dependabot).
* ⬆ Bump astral-sh/setup-uv from 4 to 5. PR [#1098](https://github.com/fastapi/typer/pull/1098) by [@dependabot[bot]](https://github.com/apps/dependabot).
* ⬆ Bump markdown-include-variants from 0.0.3 to 0.0.4. PR [#1100](https://github.com/fastapi/typer/pull/1100) by [@dependabot[bot]](https://github.com/apps/dependabot).
* ⬆ Bump ruff from 0.8.2 to 0.8.3. PR [#1090](https://github.com/fastapi/typer/pull/1090) by [@dependabot[bot]](https://github.com/apps/dependabot).
* ⬆ [pre-commit.ci] pre-commit autoupdate. PR [#1093](https://github.com/fastapi/typer/pull/1093) by [@pre-commit-ci[bot]](https://github.com/apps/pre-commit-ci).
* ⬆ Bump mkdocs-material from 9.5.48 to 9.5.49. PR [#1092](https://github.com/fastapi/typer/pull/1092) by [@dependabot[bot]](https://github.com/apps/dependabot).
* ⬆ Bump pypa/gh-action-pypi-publish from 1.12.2 to 1.12.3. PR [#1088](https://github.com/fastapi/typer/pull/1088) by [@dependabot[bot]](https://github.com/apps/dependabot).
* ⬆ [pre-commit.ci] pre-commit autoupdate. PR [#1087](https://github.com/fastapi/typer/pull/1087) by [@pre-commit-ci[bot]](https://github.com/apps/pre-commit-ci).
* ⬆ Bump ruff from 0.8.1 to 0.8.2. PR [#1084](https://github.com/fastapi/typer/pull/1084) by [@dependabot[bot]](https://github.com/apps/dependabot).
* ⬆ Bump mkdocs-material from 9.5.47 to 9.5.48. PR [#1086](https://github.com/fastapi/typer/pull/1086) by [@dependabot[bot]](https://github.com/apps/dependabot).

## 0.15.1

### Features

* 🗑️ Deprecate `shell_complete` and continue to use `autocompletion` for CLI parameters. PR [#974](https://github.com/fastapi/typer/pull/974) by [@svlandeg](https://github.com/svlandeg).

### Docs

* ✏️ Fix a few typos in the source and documentation. PR [#1028](https://github.com/fastapi/typer/pull/1028) by [@kkirsche](https://github.com/kkirsche).
* 📝 Fix minor inconsistencies and typos in tutorial. PR [#1067](https://github.com/fastapi/typer/pull/1067) by [@tvoirand](https://github.com/tvoirand).
* ✏️ Fix a few small typos in the documentation. PR [#1077](https://github.com/fastapi/typer/pull/1077) by [@svlandeg](https://github.com/svlandeg).

### Internal

* 🔧 Update build-docs filter patterns. PR [#1080](https://github.com/fastapi/typer/pull/1080) by [@tiangolo](https://github.com/tiangolo).
* 🔨 Update deploy docs preview script. PR [#1079](https://github.com/fastapi/typer/pull/1079) by [@tiangolo](https://github.com/tiangolo).
* 🔧 Update members. PR [#1078](https://github.com/fastapi/typer/pull/1078) by [@tiangolo](https://github.com/tiangolo).
* ⬆ [pre-commit.ci] pre-commit autoupdate. PR [#1071](https://github.com/fastapi/typer/pull/1071) by [@pre-commit-ci[bot]](https://github.com/apps/pre-commit-ci).
* ⬆ Update httpx requirement from <0.28.0,>=0.27.0 to >=0.27.0,<0.29.0. PR [#1065](https://github.com/fastapi/typer/pull/1065) by [@dependabot[bot]](https://github.com/apps/dependabot).

## 0.15.0

### Features

* ✨ Add support for extending typer apps without passing a name, add commands to the top level. PR [#1037](https://github.com/fastapi/typer/pull/1037) by [@patrick91](https://github.com/patrick91).
    * New docs: [One File Per Command](https://typer.tiangolo.com/tutorial/one-file-per-command/).

### Internal

* ⬆ Bump mkdocs-material from 9.5.46 to 9.5.47. PR [#1070](https://github.com/fastapi/typer/pull/1070) by [@dependabot[bot]](https://github.com/apps/dependabot).
* ⬆ Bump ruff from 0.8.0 to 0.8.1. PR [#1066](https://github.com/fastapi/typer/pull/1066) by [@dependabot[bot]](https://github.com/apps/dependabot).

## 0.14.0

### Breaking Changes

* 🔥 Remove auto naming of groups added via `add_typer` based on the group's callback function name. PR [#1052](https://github.com/fastapi/typer/pull/1052) by [@patrick91](https://github.com/patrick91).

Before, it was supported to infer the name of a command group from the callback function name in the sub-app, so, in this code:

```python
import typer

app = typer.Typer()
users_app = typer.Typer()

app.add_typer(users_app)


@users_app.callback()
def users():  # <-- This was the inferred command group name
    """
    Manage users in the app.
    """


@users_app.command()
def create(name: str):
    print(f"Creating user: {name}")
```

...the command group would be named `users`, based on the name of the function `def users()`.

Now you need to set it explicitly:

```python
import typer

app = typer.Typer()
users_app = typer.Typer()

app.add_typer(users_app, name="users")  # <-- Explicitly set the command group name


@users_app.callback()
def users():
    """
    Manage users in the app.
    """


@users_app.command()
def create(name: str):
    print(f"Creating user: {name}")
```

Updated docs [SubCommand Name and Help](https://typer.tiangolo.com/tutorial/subcommands/name-and-help/).

**Note**: this change will enable important features in the next release. 🤩

### Internal

* ⬆ Bump pypa/gh-action-pypi-publish from 1.10.3 to 1.12.2. PR [#1043](https://github.com/fastapi/typer/pull/1043) by [@dependabot[bot]](https://github.com/apps/dependabot).
* ⬆ Bump mkdocs-material from 9.5.44 to 9.5.46. PR [#1062](https://github.com/fastapi/typer/pull/1062) by [@dependabot[bot]](https://github.com/apps/dependabot).
* ⬆ Bump ruff from 0.7.4 to 0.8.0. PR [#1059](https://github.com/fastapi/typer/pull/1059) by [@dependabot[bot]](https://github.com/apps/dependabot).
* ⬆ Bump astral-sh/setup-uv from 3 to 4. PR [#1061](https://github.com/fastapi/typer/pull/1061) by [@dependabot[bot]](https://github.com/apps/dependabot).
* ⬆ [pre-commit.ci] pre-commit autoupdate. PR [#1053](https://github.com/fastapi/typer/pull/1053) by [@pre-commit-ci[bot]](https://github.com/apps/pre-commit-ci).

## 0.13.1

### Features

* ✨ Remove Rich tags when showing completion text. PR [#877](https://github.com/fastapi/typer/pull/877) by [@svlandeg](https://github.com/svlandeg).
* ✨ Render Rich markup as HTML in Markdown docs. PR [#847](https://github.com/fastapi/typer/pull/847) by [@svlandeg](https://github.com/svlandeg).
* ✨ Support cp850 encoding for auto-completion in PowerShell. PR [#808](https://github.com/fastapi/typer/pull/808) by [@svlandeg](https://github.com/svlandeg).
* ✨ Allow gettext translation of help message. PR [#886](https://github.com/fastapi/typer/pull/886) by [@svlandeg](https://github.com/svlandeg).

### Refactors

* 🐛 Fix printing HTML from Rich output. PR [#1055](https://github.com/fastapi/typer/pull/1055) by [@tiangolo](https://github.com/tiangolo).

### Docs

* 📝 Update markdown includes to use the new simpler format. PR [#1054](https://github.com/fastapi/typer/pull/1054) by [@tiangolo](https://github.com/tiangolo).

### Internal

* ⬆ Bump ruff from 0.7.3 to 0.7.4. PR [#1051](https://github.com/fastapi/typer/pull/1051) by [@dependabot[bot]](https://github.com/apps/dependabot).
* ⬆ [pre-commit.ci] pre-commit autoupdate. PR [#1047](https://github.com/fastapi/typer/pull/1047) by [@pre-commit-ci[bot]](https://github.com/apps/pre-commit-ci).
* ⬆ Bump ruff from 0.7.2 to 0.7.3. PR [#1046](https://github.com/fastapi/typer/pull/1046) by [@dependabot[bot]](https://github.com/apps/dependabot).
* ⬆ Bump tiangolo/latest-changes from 0.3.1 to 0.3.2. PR [#1044](https://github.com/fastapi/typer/pull/1044) by [@dependabot[bot]](https://github.com/apps/dependabot).
* ⬆ Update pytest-cov requirement from <6.0.0,>=2.10.0 to >=2.10.0,<7.0.0. PR [#1033](https://github.com/fastapi/typer/pull/1033) by [@dependabot[bot]](https://github.com/apps/dependabot).

## 0.13.0

### Features

* ✨ Handle `KeyboardInterrupt` separately from other exceptions. PR [#1039](https://github.com/fastapi/typer/pull/1039) by [@patrick91](https://github.com/patrick91).
* ✨ Update `launch` to not print anything when opening urls. PR [#1035](https://github.com/fastapi/typer/pull/1035) by [@patrick91](https://github.com/patrick91).
* ✨ Show help items in order of definition. PR [#944](https://github.com/fastapi/typer/pull/944) by [@svlandeg](https://github.com/svlandeg).

### Fixes

* 🐛 Fix equality check for custom classes. PR [#979](https://github.com/fastapi/typer/pull/979) by [@AryazE](https://github.com/AryazE).
* 🐛 Allow colon in zsh autocomplete values and descriptions. PR [#988](https://github.com/fastapi/typer/pull/988) by [@snapbug](https://github.com/snapbug).

### Refactors

* 🗑️ Deprecate support for `is_flag` and `flag_value` parameters. PR [#987](https://github.com/fastapi/typer/pull/987) by [@svlandeg](https://github.com/svlandeg).
* 🔥 Remove unused functionality from `_typing.py` file. PR [#805](https://github.com/fastapi/typer/pull/805) by [@ivantodorovich](https://github.com/ivantodorovich).
* ✏️ Fix typo in function name `_make_rich_text`. PR [#959](https://github.com/fastapi/typer/pull/959) by [@svlandeg](https://github.com/svlandeg).

### Internal

* ✅ Only run completion installation tests when the env var `_TYPER_RUN_INSTALL_COMPLETION_TESTS` is set. PR [#995](https://github.com/fastapi/typer/pull/995) by [@svlandeg](https://github.com/svlandeg).
* 📝 Update the docstring of the `_make_rich_text` method. PR [#972](https://github.com/fastapi/typer/pull/972) by [@svlandeg](https://github.com/svlandeg).
* ⬆ [pre-commit.ci] pre-commit autoupdate. PR [#1040](https://github.com/fastapi/typer/pull/1040) by [@pre-commit-ci[bot]](https://github.com/apps/pre-commit-ci).
* ⬆ Bump mkdocs-material from 9.5.42 to 9.5.44. PR [#1042](https://github.com/fastapi/typer/pull/1042) by [@dependabot[bot]](https://github.com/apps/dependabot).
* ⬆ Bump ruff from 0.7.1 to 0.7.2. PR [#1038](https://github.com/fastapi/typer/pull/1038) by [@dependabot[bot]](https://github.com/apps/dependabot).
* ⬆ Bump mkdocs-macros-plugin from 1.3.6 to 1.3.7. PR [#1031](https://github.com/fastapi/typer/pull/1031) by [@dependabot[bot]](https://github.com/apps/dependabot).
* ⬆ [pre-commit.ci] pre-commit autoupdate. PR [#1032](https://github.com/fastapi/typer/pull/1032) by [@pre-commit-ci[bot]](https://github.com/apps/pre-commit-ci).
* ⬆ Bump ruff from 0.7.0 to 0.7.1. PR [#1029](https://github.com/fastapi/typer/pull/1029) by [@dependabot[bot]](https://github.com/apps/dependabot).
* ⬆ Bump pillow from 10.4.0 to 11.0.0. PR [#1023](https://github.com/fastapi/typer/pull/1023) by [@dependabot[bot]](https://github.com/apps/dependabot).
* ⬆ Bump mkdocs-material from 9.5.35 to 9.5.42. PR [#1027](https://github.com/fastapi/typer/pull/1027) by [@dependabot[bot]](https://github.com/apps/dependabot).
* ⬆ Bump ruff from 0.6.5 to 0.7.0. PR [#1026](https://github.com/fastapi/typer/pull/1026) by [@dependabot[bot]](https://github.com/apps/dependabot).
* ⬆ Bump mkdocs-macros-plugin from 1.2.0 to 1.3.6. PR [#1025](https://github.com/fastapi/typer/pull/1025) by [@dependabot[bot]](https://github.com/apps/dependabot).
* ⬆ Update pre-commit requirement from <4.0.0,>=2.17.0 to >=2.17.0,<5.0.0. PR [#1012](https://github.com/fastapi/typer/pull/1012) by [@dependabot[bot]](https://github.com/apps/dependabot).
* ⬆ Bump pypa/gh-action-pypi-publish from 1.10.1 to 1.10.3. PR [#1009](https://github.com/fastapi/typer/pull/1009) by [@dependabot[bot]](https://github.com/apps/dependabot).
* ⬆ [pre-commit.ci] pre-commit autoupdate. PR [#1001](https://github.com/fastapi/typer/pull/1001) by [@pre-commit-ci[bot]](https://github.com/apps/pre-commit-ci).
* 👷 Update Deploy docs CI to use uv. PR [#1021](https://github.com/fastapi/typer/pull/1021) by [@tiangolo](https://github.com/tiangolo).
* 👷 Fix smokeshow, checkout files on CI. PR [#1020](https://github.com/fastapi/typer/pull/1020) by [@tiangolo](https://github.com/tiangolo).
* 👷 Use uv in CI. PR [#1019](https://github.com/fastapi/typer/pull/1019) by [@tiangolo](https://github.com/tiangolo).
* 👷 Update `labeler.yml`. PR [#1014](https://github.com/fastapi/typer/pull/1014) by [@tiangolo](https://github.com/tiangolo).
* 👷 Update worfkow deploy-docs-notify URL. PR [#1011](https://github.com/fastapi/typer/pull/1011) by [@tiangolo](https://github.com/tiangolo).
* 👷 Upgrade Cloudflare GitHub Action. PR [#1010](https://github.com/fastapi/typer/pull/1010) by [@tiangolo](https://github.com/tiangolo).
* ⬆ Bump mkdocs-macros-plugin from 1.0.5 to 1.2.0. PR [#992](https://github.com/fastapi/typer/pull/992) by [@dependabot[bot]](https://github.com/apps/dependabot).
* ⬆ Bump ruff from 0.6.4 to 0.6.5. PR [#991](https://github.com/fastapi/typer/pull/991) by [@dependabot[bot]](https://github.com/apps/dependabot).
* ⬆ Bump mkdocs-material from 9.5.34 to 9.5.35. PR [#996](https://github.com/fastapi/typer/pull/996) by [@dependabot[bot]](https://github.com/apps/dependabot).
* ⬆ [pre-commit.ci] pre-commit autoupdate. PR [#993](https://github.com/fastapi/typer/pull/993) by [@pre-commit-ci[bot]](https://github.com/apps/pre-commit-ci).
* ⬆ [pre-commit.ci] pre-commit autoupdate. PR [#982](https://github.com/fastapi/typer/pull/982) by [@pre-commit-ci[bot]](https://github.com/apps/pre-commit-ci).
* ⬆ Bump tiangolo/issue-manager from 0.5.0 to 0.5.1. PR [#980](https://github.com/fastapi/typer/pull/980) by [@dependabot[bot]](https://github.com/apps/dependabot).
* 👷 Update `issue-manager.yml`. PR [#978](https://github.com/fastapi/typer/pull/978) by [@tiangolo](https://github.com/tiangolo).
* ⬆ Bump ruff from 0.6.3 to 0.6.4. PR [#975](https://github.com/fastapi/typer/pull/975) by [@dependabot[bot]](https://github.com/apps/dependabot).
* ⬆ Bump mkdocs-material from 9.5.33 to 9.5.34. PR [#963](https://github.com/fastapi/typer/pull/963) by [@dependabot[bot]](https://github.com/apps/dependabot).
* ⬆ Bump pypa/gh-action-pypi-publish from 1.9.0 to 1.10.1. PR [#973](https://github.com/fastapi/typer/pull/973) by [@dependabot[bot]](https://github.com/apps/dependabot).
* ⬆ [pre-commit.ci] pre-commit autoupdate. PR [#966](https://github.com/fastapi/typer/pull/966) by [@pre-commit-ci[bot]](https://github.com/apps/pre-commit-ci).
* 💚 Set `include-hidden-files` to `True` when using the `upload-artifact` GH action. PR [#967](https://github.com/fastapi/typer/pull/967) by [@svlandeg](https://github.com/svlandeg).
* ⬆ Bump ruff from 0.6.1 to 0.6.3. PR [#961](https://github.com/fastapi/typer/pull/961) by [@dependabot[bot]](https://github.com/apps/dependabot).
* ⬆ [pre-commit.ci] pre-commit autoupdate. PR [#689](https://github.com/fastapi/typer/pull/689) by [@pre-commit-ci[bot]](https://github.com/apps/pre-commit-ci).
* ⬆ Bump ruff from 0.2.0 to 0.6.1. PR [#938](https://github.com/fastapi/typer/pull/938) by [@dependabot[bot]](https://github.com/apps/dependabot).
* 👷 Update `latest-changes` GitHub Action. PR [#955](https://github.com/fastapi/typer/pull/955) by [@tiangolo](https://github.com/tiangolo).

## 0.12.5

### Features

* 💄 Unify the width of the Rich console for help and errors. PR [#788](https://github.com/fastapi/typer/pull/788) by [@racinmat](https://github.com/racinmat).
* 🚸 Improve assertion error message if a group is not a valid subclass. PR [#425](https://github.com/fastapi/typer/pull/425) by [@chrisburr](https://github.com/chrisburr).

### Fixes

* 🐛 Ensure `rich_markup_mode=None` disables Rich formatting. PR [#859](https://github.com/fastapi/typer/pull/859) by [@svlandeg](https://github.com/svlandeg).
* 🐛  Fix sourcing of completion path for Git Bash. PR [#801](https://github.com/fastapi/typer/pull/801) by [@svlandeg](https://github.com/svlandeg).
* 🐛 Fix PowerShell completion with incomplete word. PR [#360](https://github.com/fastapi/typer/pull/360) by [@patricksurry](https://github.com/patricksurry).

### Refactors

* 🔥 Remove Python 3.6 specific code paths. PR [#850](https://github.com/fastapi/typer/pull/850) by [@svlandeg](https://github.com/svlandeg).
* 🔥 Clean up redundant code. PR [#858](https://github.com/fastapi/typer/pull/858) by [@svlandeg](https://github.com/svlandeg).

### Docs

* ♻️ Use F-strings in Click examples in docs. PR [#891](https://github.com/fastapi/typer/pull/891) by [@svlandeg](https://github.com/svlandeg).
* 📝Add missing `main.py` in tutorial on CLI option names. PR [#868](https://github.com/fastapi/typer/pull/868) by [@fsramalho](https://github.com/fsramalho).
* 📝 Fix broken link. PR [#835](https://github.com/fastapi/typer/pull/835) by [@OhioDschungel6](https://github.com/OhioDschungel6).
* 📝 Update package docs with the latest versions of Typer and Poetry. PR [#781](https://github.com/fastapi/typer/pull/781) by [@kinuax](https://github.com/kinuax).
* 📝 Update the Progress Bar tutorial with correct output. PR [#199](https://github.com/fastapi/typer/pull/199) by [@n1ckdm](https://github.com/n1ckdm).
* 📝 Add docs and scripts to test completion in different shells. PR [#953](https://github.com/fastapi/typer/pull/953) by [@tiangolo](https://github.com/tiangolo).
* ✏️ Fix a typo in `docs/virtual-environments.md`. PR [#952](https://github.com/fastapi/typer/pull/952) by [@tiangolo](https://github.com/tiangolo).
* ✏️ Fix typo in `docs/contributing.md`. PR [#947](https://github.com/fastapi/typer/pull/947) by [@tiangolo](https://github.com/tiangolo).
* 📝 Add docs for virtual environments, environment variables, and update contributing. PR [#946](https://github.com/fastapi/typer/pull/946) by [@tiangolo](https://github.com/tiangolo).

### Internal

* 🔨 Pre-install dependencies in Docker so that testing in Docker is faster. PR [#954](https://github.com/fastapi/typer/pull/954) by [@tiangolo](https://github.com/tiangolo).
* ✅ Add `needs_bash` test fixture. PR [#888](https://github.com/fastapi/typer/pull/888) by [@svlandeg](https://github.com/svlandeg).
* ⬆ Bump mkdocs-material from 9.5.18 to 9.5.33. PR [#945](https://github.com/fastapi/typer/pull/945) by [@dependabot[bot]](https://github.com/apps/dependabot).
* ⬆ Bump pillow from 10.3.0 to 10.4.0. PR [#939](https://github.com/fastapi/typer/pull/939) by [@dependabot[bot]](https://github.com/apps/dependabot).
* 👷 Fix issue-manager. PR [#948](https://github.com/fastapi/typer/pull/948) by [@tiangolo](https://github.com/tiangolo).
* 🙈 Remove extra line in .gitignore. PR [#936](https://github.com/fastapi/typer/pull/936) by [@tiangolo](https://github.com/tiangolo).
* ⬆ Update pytest-cov requirement from <5.0.0,>=2.10.0 to >=2.10.0,<6.0.0. PR [#844](https://github.com/fastapi/typer/pull/844) by [@dependabot[bot]](https://github.com/apps/dependabot).
* ⬆ Bump pypa/gh-action-pypi-publish from 1.8.11 to 1.9.0. PR [#865](https://github.com/fastapi/typer/pull/865) by [@dependabot[bot]](https://github.com/apps/dependabot).
* ⬆ Update pytest requirement from <8.0.0,>=4.4.0 to >=4.4.0,<9.0.0. PR [#915](https://github.com/fastapi/typer/pull/915) by [@dependabot[bot]](https://github.com/apps/dependabot).
* ⬆ Update pytest-sugar requirement from <0.10.0,>=0.9.4 to >=0.9.4,<1.1.0. PR [#841](https://github.com/fastapi/typer/pull/841) by [@dependabot[bot]](https://github.com/apps/dependabot).

## 0.12.4

### Features

* ✨ Add support for Python 3.12, tests in CI and official marker. PR [#807](https://github.com/tiangolo/typer/pull/807) by [@ivantodorovich](https://github.com/ivantodorovich).

### Fixes

* 🐛 Fix support for `UnionType` (e.g. `str | None`) with Python 3.11. PR [#548](https://github.com/fastapi/typer/pull/548) by [@jonaslb](https://github.com/jonaslb).
* 🐛 Fix `zsh` autocompletion installation. PR [#237](https://github.com/fastapi/typer/pull/237) by [@alexjurkiewicz](https://github.com/alexjurkiewicz).
* 🐛 Fix usage of `Annotated` with future annotations in Python 3.7+. PR [#814](https://github.com/fastapi/typer/pull/814) by [@ivantodorovich](https://github.com/ivantodorovich).
* 🐛 Fix `shell_complete` not working for Arguments. PR [#737](https://github.com/fastapi/typer/pull/737) by [@bckohan](https://github.com/bckohan).

### Docs

* 📝 Update docs links, from tiangolo to new fastapi org. PR [#919](https://github.com/fastapi/typer/pull/919) by [@tiangolo](https://github.com/tiangolo).
* 📝 Add docs for team and repo management. PR [#917](https://github.com/tiangolo/typer/pull/917) by [@tiangolo](https://github.com/tiangolo).

### Internal

* 🔧 Add URLs to `pyproject.toml`, show up in PyPI. PR [#931](https://github.com/fastapi/typer/pull/931) by [@tiangolo](https://github.com/tiangolo).
* 👷 Do not sync labels as it overrides manually added labels. PR [#930](https://github.com/fastapi/typer/pull/930) by [@tiangolo](https://github.com/tiangolo).
* 👷 Update labeler GitHub Action to add only one label. PR [#927](https://github.com/fastapi/typer/pull/927) by [@tiangolo](https://github.com/tiangolo).
* 👷 Update labeler GitHub Actions permissions and dependencies. PR [#926](https://github.com/fastapi/typer/pull/926) by [@tiangolo](https://github.com/tiangolo).
* 👷 Add GitHub Action label-checker. PR [#925](https://github.com/fastapi/typer/pull/925) by [@tiangolo](https://github.com/tiangolo).
* 👷 Add GitHub Action labeler. PR [#924](https://github.com/fastapi/typer/pull/924) by [@tiangolo](https://github.com/tiangolo).
* 👷 Add GitHub Action add-to-project. PR [#922](https://github.com/fastapi/typer/pull/922) by [@tiangolo](https://github.com/tiangolo).
* 🔨 Update docs.py script to enable dirty reload conditionally. PR [#918](https://github.com/tiangolo/typer/pull/918) by [@tiangolo](https://github.com/tiangolo).
* 🔧 Update MkDocs previews. PR [#916](https://github.com/tiangolo/typer/pull/916) by [@tiangolo](https://github.com/tiangolo).
* 👷 Upgrade build docs configs. PR [#914](https://github.com/tiangolo/typer/pull/914) by [@tiangolo](https://github.com/tiangolo).
* 🔧 Update MkDocs to have titles in Markdown files instead of config. PR [#913](https://github.com/tiangolo/typer/pull/913) by [@tiangolo](https://github.com/tiangolo).
* 👷 Add alls-green for test-redistribute. PR [#911](https://github.com/tiangolo/typer/pull/911) by [@tiangolo](https://github.com/tiangolo).
* 👷 Update docs-previews to handle no docs changes. PR [#912](https://github.com/tiangolo/typer/pull/912) by [@tiangolo](https://github.com/tiangolo).
* 👷🏻 Show docs deployment status and preview URLs in comment. PR [#910](https://github.com/tiangolo/typer/pull/910) by [@tiangolo](https://github.com/tiangolo).
* 🔧 Enable auto dark mode from system. PR [#908](https://github.com/tiangolo/typer/pull/908) by [@tiangolo](https://github.com/tiangolo).
* 💄 Add dark mode logo. PR [#907](https://github.com/tiangolo/typer/pull/907) by [@tiangolo](https://github.com/tiangolo).
* 🔧 Update tabs and admonitions with new syntax and new MkDocs features. PR [#906](https://github.com/tiangolo/typer/pull/906) by [@tiangolo](https://github.com/tiangolo).
* 🔧 Enable MkDocs Material features. PR [#905](https://github.com/tiangolo/typer/pull/905) by [@tiangolo](https://github.com/tiangolo).
* 🔧 Enable dark mode for docs. PR [#904](https://github.com/tiangolo/typer/pull/904) by [@tiangolo](https://github.com/tiangolo).
* ➖ Do not install jieba for MkDocs Material as there are no chinese translations. PR [#903](https://github.com/tiangolo/typer/pull/903) by [@tiangolo](https://github.com/tiangolo).
* 🙈 Add MkDocs Material cache to gitignore. PR [#902](https://github.com/tiangolo/typer/pull/902) by [@tiangolo](https://github.com/tiangolo).
* 🔨 Update lint script. PR [#901](https://github.com/tiangolo/typer/pull/901) by [@tiangolo](https://github.com/tiangolo).
* 🔧 Update MkDocs configs and docs build setup. PR [#900](https://github.com/tiangolo/typer/pull/900) by [@tiangolo](https://github.com/tiangolo).
* ⬆ Bump actions/cache from 3 to 4. PR [#839](https://github.com/tiangolo/typer/pull/839) by [@dependabot[bot]](https://github.com/apps/dependabot).
* 🍱 Update Typer icon and logo. PR [#899](https://github.com/tiangolo/typer/pull/899) by [@tiangolo](https://github.com/tiangolo).
* 👷 Update issue-manager.yml GitHub Action permissions. PR [#897](https://github.com/tiangolo/typer/pull/897) by [@tiangolo](https://github.com/tiangolo).
* 👷 Refactor GitHub Action to comment docs deployment URLs and update token, preparing for GitHub org. PR [#896](https://github.com/tiangolo/typer/pull/896) by [@tiangolo](https://github.com/tiangolo).
* 🔨 Update docs Termynal scripts to not include line nums for local dev. PR [#882](https://github.com/tiangolo/typer/pull/882) by [@tiangolo](https://github.com/tiangolo).
* ⬆ Bump black from 23.3.0 to 24.3.0. PR [#837](https://github.com/tiangolo/typer/pull/837) by [@dependabot[bot]](https://github.com/apps/dependabot).
* ⬆ Bump pillow from 10.1.0 to 10.3.0. PR [#836](https://github.com/tiangolo/typer/pull/836) by [@dependabot[bot]](https://github.com/apps/dependabot).
* ✅ Add CI configs to run tests on Windows and MacOS. PR [#824](https://github.com/tiangolo/typer/pull/824) by [@svlandeg](https://github.com/svlandeg).
* 👷 Update GitHub Actions to upload and download artifacts. PR [#829](https://github.com/tiangolo/typer/pull/829) by [@tiangolo](https://github.com/tiangolo).
* 👷 Tweak CI for test-redistribute, add needed env vars for slim. PR [#827](https://github.com/tiangolo/typer/pull/827) by [@tiangolo](https://github.com/tiangolo).
* ✅ Generalize test suite to run on Windows. PR [#810](https://github.com/tiangolo/typer/pull/810) by [@svlandeg](https://github.com/svlandeg).
* ✅ Add `__init__.py` files to fix test suite. PR [#809](https://github.com/tiangolo/typer/pull/809) by [@svlandeg](https://github.com/svlandeg).
* 🔧 Update MkDocs Material, enable plugins. PR [#813](https://github.com/tiangolo/typer/pull/813) by [@tiangolo](https://github.com/tiangolo).
* 🔧 Tweak development scripts and configs after migration to PDM, Ruff, etc.. PR [#797](https://github.com/tiangolo/typer/pull/797) by [@tiangolo](https://github.com/tiangolo).

## 0.12.3

### Fixes

* 🐛 Fix Rich formatting with no commands. PR [#796](https://github.com/tiangolo/typer/pull/796) by [@svlandeg](https://github.com/svlandeg).

## 0.12.2

### Features

* ✨ Improve column help display, ensure commands column width is the same on all panels. PR [#567](https://github.com/tiangolo/typer/pull/567) by [@ssbarnea](https://github.com/ssbarnea).

### Fixes

* 🐛 Add support for an argument of type `Optional[Tuple]` and default value `None`. PR [#757](https://github.com/tiangolo/typer/pull/757) by [@Asthestarsfalll](https://github.com/Asthestarsfalll).

### Docs

* 🔧 Fix typo in Github template. PR [#793](https://github.com/tiangolo/typer/pull/793) by [@svlandeg](https://github.com/svlandeg).
* 📝 Fix typos in documentation. PR [#761](https://github.com/tiangolo/typer/pull/761) by [@svlandeg](https://github.com/svlandeg).
* 📝 Update console output with Click 8 messages. PR [#789](https://github.com/tiangolo/typer/pull/789) by [@svlandeg](https://github.com/svlandeg).
* 📝 Remove references to a .rst README generated by poetry new. PR [#632](https://github.com/tiangolo/typer/pull/632) by [@jonasmmiguel](https://github.com/jonasmmiguel).

## 0.12.1

Now you don't need to install `typer[all]`. When you install `typer` it comes with the default optional dependencies and the `typer` command.

If you don't want the extra optional dependencies (`rich` and `shellingham`), you can install `typer-slim` instead.

You can also install `typer-slim[standard]`, which includes the default optional dependencies, but not the `typer` command.

Now the package `typer-cli` doesn't add anything on top of what `typer` has, it only depends on `typer`, and is there only for backwards compatibility, so that projects that depend on `typer-cli` can get the latest features of the `typer` command while they upgrade their dependencies to require `typer` directly.

### Features

* ✨ Add support for `typer ./someprogram.py utils docs --title`. PR [#782](https://github.com/tiangolo/typer/pull/782) by [@tiangolo](https://github.com/tiangolo).

### Fixes

* 🐛 Fix broken installation when upgrading from `typer <0.12.0` to `typer >=0.12.0`, make `typer` independent of `typer-slim`, include `typer` command in `typer` package. PR [#791](https://github.com/tiangolo/typer/pull/791) by [@tiangolo](https://github.com/tiangolo).

This fixes a problem that would break the `typer` installation directory when upgrading from `typer <0.12.0` to `typer >=0.12.0`, see issue [#790](https://github.com/tiangolo/typer/issues/790).

By installing the latest version (`0.12.1`) it fixes it, for any previous version, even if the installation directory was already broken by the previous upgrade.

### Internal

* 👷 Add cron to run test once a week on monday. PR [#783](https://github.com/tiangolo/typer/pull/783) by [@estebanx64](https://github.com/estebanx64).

## 0.12.0

In version `0.12.0`, the `typer` package depends on `typer-slim[standard]` which includes the default dependencies (instead of `typer[all]`) and `typer-cli` (that provides the `typer` command).

If you don't want the extra optional dependencies (`rich` and `shellingham`), you can install `typer-slim` instead.

You can also install `typer-slim[standard]`, which includes the default optional dependencies, but not the `typer` command.

In version `0.12.0` the `typer-cli` package only provides the `typer` command, but the code is still in the main code, so even without installing `typer-cli`, it can be called with `python -m typer`.

This approach of having `typer` depend on `typer-slim[standard]` instead of including the whole code and dependencies itself caused an issue when upgrading from `typer <0.12.0` to `typer >=0.12.0`, see issue [#790](https://github.com/tiangolo/typer/issues/790). This is fixed in version `0.12.1`.

### Features

* ✨ Add `typer-slim` package without extras, make `typer` include `typer-slim[default]` and integrate Typer CLI (`typer` command) into Typer. PR [#780](https://github.com/tiangolo/typer/pull/780) by [@tiangolo](https://github.com/tiangolo).

### Internal

* 🔧 Temporarily disable social plugin while a MkDocs issue is handled. PR [#779](https://github.com/tiangolo/typer/pull/779) by [@tiangolo](https://github.com/tiangolo).
* 👷 Fix install MkDocs Insiders only when available. PR [#778](https://github.com/tiangolo/typer/pull/778) by [@tiangolo](https://github.com/tiangolo).

## 0.11.1

### Fixes

* 🔧 Explicitly include testing files in sdist for redistributors (e.g. OpenSUSE) and add CI to test redistribution. PR [#773](https://github.com/tiangolo/typer/pull/773) by [@tiangolo](https://github.com/tiangolo).

### Internal

* 👷 Do not use the cache for dependencies when publishing to PyPI. PR [#774](https://github.com/tiangolo/typer/pull/774) by [@tiangolo](https://github.com/tiangolo).

## 0.11.0

### Breaking Changes

* 🔧 Refactor package manager, move from Flit to PDM, remove private pip extras for `test`, `doc`, `dev`. PR [#764](https://github.com/tiangolo/typer/pull/764) by [@tiangolo](https://github.com/tiangolo).
* 🔥 Remove support for Click 7, require Click 8+. PR [#760](https://github.com/tiangolo/typer/pull/760) by [@tiangolo](https://github.com/tiangolo).
* 🔥 Remove support for Python 3.6. PR [#758](https://github.com/tiangolo/typer/pull/758) by [@tiangolo](https://github.com/tiangolo).

### Refactors

* 🔧 Migrate from Black, isort, flake8, autoflake, pyupgrade to Ruff. PR [#763](https://github.com/tiangolo/typer/pull/763) by [@tiangolo](https://github.com/tiangolo).

### Internal

* ⬆️ Upgrade coverage and configs. PR [#769](https://github.com/tiangolo/typer/pull/769) by [@tiangolo](https://github.com/tiangolo).
* 🔧 Upgrade mypy and config. PR [#768](https://github.com/tiangolo/typer/pull/768) by [@tiangolo](https://github.com/tiangolo).
* 👷 Upgrade Smokeshow GitHub action. PR [#767](https://github.com/tiangolo/typer/pull/767) by [@tiangolo](https://github.com/tiangolo).
* 👷 Upgrade latest-changes GitHub Action. PR [#766](https://github.com/tiangolo/typer/pull/766) by [@tiangolo](https://github.com/tiangolo).
* 👷 Upgrade issue-manager GitHub Action. PR [#765](https://github.com/tiangolo/typer/pull/765) by [@tiangolo](https://github.com/tiangolo).
* 👷 Add alls-green to CI. PR [#759](https://github.com/tiangolo/typer/pull/759) by [@tiangolo](https://github.com/tiangolo).

## 0.10.0

### Fixes

* 🐛 Fix default value of `None` for CLI Parameters when the type is `list | None` and the default value is `None`. PR [#664](https://github.com/tiangolo/typer/pull/664) by [@theowisear](https://github.com/theowisear).

## 0.9.4

### Features

* ✨ Improve support for CLI translations using gettext. PR [#417](https://github.com/tiangolo/typer/pull/417) by [@mjodmj](https://github.com/mjodmj).

## 0.9.3

### Fixes

* 🐛 Fix evaluating stringified annotations in Python 3.10 (also `from __future__ import annotations`). PR [#721](https://github.com/tiangolo/typer/pull/721) by [@heckad](https://github.com/heckad).

## 0.9.2

### Fixes

* 🐛 Fix display of default value for Enum parameters inside of a list, include docs and tests. PR [#473](https://github.com/tiangolo/typer/pull/473) by [@asieira](https://github.com/asieira).
* 🐛 Update type annotations for `show_default` parameter and update docs for setting a "Custom default string". PR [#501](https://github.com/tiangolo/typer/pull/501) by [@plannigan](https://github.com/plannigan).

### Docs

* 📝 Add docs and test for `no_args_is_help` feature. PR [#751](https://github.com/tiangolo/typer/pull/751) by [@svlandeg](https://github.com/svlandeg).

## 0.9.1

### Fixes

* 🐛 Add missing `default_factory` in `Argument` overloads. PR [#750](https://github.com/tiangolo/typer/pull/750) by [@m9810223](https://github.com/m9810223).
* 🐛 Fix preserving case in enum values. PR [#571](https://github.com/tiangolo/typer/pull/571) by [@avaldebe](https://github.com/avaldebe).

### Docs

* 📝 Remove obsolete references to `--install-completion` for `typer.run()` scripts. PR [#595](https://github.com/tiangolo/typer/pull/595) by [@tiangolo](https://github.com/tiangolo).

* 📝 Update docs example for a Typer/Click group to make new subcommands explicit. PR [#755](https://github.com/tiangolo/typer/pull/755) by [@svlandeg](https://github.com/svlandeg).
* 📝 Update docs for building a package, file structure example. PR [#683](https://github.com/tiangolo/typer/pull/683) by [@davidbgk](https://github.com/davidbgk).
* 📝 Update link in docs to the newest stable version of click. PR [#675](https://github.com/tiangolo/typer/pull/675) by [@javier171188](https://github.com/javier171188).
* 🔧 Add `CITATION.cff` file for academic citations. PR [#681](https://github.com/tiangolo/typer/pull/681) by [@tiangolo](https://github.com/tiangolo).
* ✏ Fix typo in `docs/tutorial/exceptions.md`. PR [#702](https://github.com/tiangolo/typer/pull/702) by [@menzenski](https://github.com/menzenski).
* ✏ Fix typo in `docs/tutorial/options/name.md`. PR [#725](https://github.com/tiangolo/typer/pull/725) by [@bwagner](https://github.com/bwagner).
* ✏ Fix typo in `docs/tutorial/arguments/optional.md`. PR [#602](https://github.com/tiangolo/typer/pull/602) by [@tadasgedgaudas](https://github.com/tadasgedgaudas).

### Internal

* ⬆ [pre-commit.ci] pre-commit autoupdate. PR [#606](https://github.com/tiangolo/typer/pull/606) by [@pre-commit-ci[bot]](https://github.com/apps/pre-commit-ci).
* 👷 Install MkDocs Material Insiders only when secrets are available, for Dependabot. PR [#685](https://github.com/tiangolo/typer/pull/685) by [@tiangolo](https://github.com/tiangolo).
* ⚒️ Update build-docs.yml, do not zip docs. PR [#645](https://github.com/tiangolo/typer/pull/645) by [@tiangolo](https://github.com/tiangolo).
* 👷 Deploy docs to Cloudflare. PR [#644](https://github.com/tiangolo/typer/pull/644) by [@tiangolo](https://github.com/tiangolo).
* 👷 Upgrade CI for docs. PR [#642](https://github.com/tiangolo/typer/pull/642) by [@tiangolo](https://github.com/tiangolo).
* 👷 Update token for latest changes. PR [#635](https://github.com/tiangolo/typer/pull/635) by [@tiangolo](https://github.com/tiangolo).
* 👷 Update CI workflow dispatch for latest changes. PR [#643](https://github.com/tiangolo/typer/pull/643) by [@tiangolo](https://github.com/tiangolo).
* 👷 Update token for Material for MkDocs Insiders. PR [#636](https://github.com/tiangolo/typer/pull/636) by [@tiangolo](https://github.com/tiangolo).
* 🐛 Fix internal type annotations and bump mypy version. PR [#638](https://github.com/tiangolo/typer/pull/638) by [@paulo-raca](https://github.com/paulo-raca).
* 💡 Add comments to document overload definitions in code. PR [#752](https://github.com/tiangolo/typer/pull/752) by [@svlandeg](https://github.com/svlandeg).
* 🔥 Remove Jina QA Bot as it has been discontinued. PR [#749](https://github.com/tiangolo/typer/pull/749) by [@tiangolo](https://github.com/tiangolo).
* 👷 Update build docs CI cache paths. PR [#707](https://github.com/tiangolo/typer/pull/707) by [@tiangolo](https://github.com/tiangolo).
* 👷 Upgrade latest-changes GitHub Action. PR [#691](https://github.com/tiangolo/typer/pull/691) by [@tiangolo](https://github.com/tiangolo).

## 0.9.0

### Features

* ✨ Add support for PEP-593 `Annotated` for specifying options and arguments. Initial PR [#584](https://github.com/tiangolo/typer/pull/584) by [@ryangalamb](https://github.com/ryangalamb).
    * New docs: [Optional CLI arguments](https://typer.tiangolo.com/tutorial/arguments/optional/#an-alternative-cli-argument-declaration).
    * It is no longer required to pass a default value of `...` to mark a *CLI Argument* or *CLI Option* as required.
    * It is now recommended to use `Annotated` for `typer.Option()` and `typer.Argument()`.
    * All the docs have been updated to recommend `Annotated`.

### Docs

* 📝 Update docs examples for custom param types using `Annotated`, fix overloads for `typer.Argument`. PR [#594](https://github.com/tiangolo/typer/pull/594) by [@tiangolo](https://github.com/tiangolo).

### Internal

* ⬆ [pre-commit.ci] pre-commit autoupdate. PR [#592](https://github.com/tiangolo/typer/pull/592) by [@pre-commit-ci[bot]](https://github.com/apps/pre-commit-ci).

## 0.8.0

### Features

* ✨ Add support for custom types and parsers. Initial PR [#583](https://github.com/tiangolo/typer/pull/583) by [@jpurviance](https://github.com/jpurviance). Based on original PR [#443](https://github.com/tiangolo/typer/pull/443) by [@paulo-raca](https://github.com/paulo-raca).
    * New docs: [CLI Parameter Types: Custom Types](https://typer.tiangolo.com/tutorial/parameter-types/custom-types/).

### Upgrades

* ⬆ Upgrade Rich, support 13.x. PR [#524](https://github.com/tiangolo/typer/pull/524) by [@musicinmybrain](https://github.com/musicinmybrain).

### Docs

* 📝 Tweak docs, Custom Types path, main page and READAME colors, broken links. PR [#588](https://github.com/tiangolo/typer/pull/588) by [@tiangolo](https://github.com/tiangolo).
* ✏ Fix spelling (shinny -> shiny). PR [#586](https://github.com/tiangolo/typer/pull/586) by [@runofthemill](https://github.com/runofthemill).
* 📝 Update docs about helping Typer. PR [#547](https://github.com/tiangolo/typer/pull/547) by [@tiangolo](https://github.com/tiangolo).
* ✏️ Fix typo in datetime docs. PR [#495](https://github.com/tiangolo/typer/pull/495) by [@huxuan](https://github.com/huxuan).
* ✏️ Add quotes to package name that includes brackets in docs. PR [#475](https://github.com/tiangolo/typer/pull/475) by [@gjolga](https://github.com/gjolga).

### Internal

* ⬆ Bump dawidd6/action-download-artifact from 2.24.2 to 2.26.0. PR [#558](https://github.com/tiangolo/typer/pull/558) by [@dependabot[bot]](https://github.com/apps/dependabot).
* ⬆ [pre-commit.ci] pre-commit autoupdate. PR [#549](https://github.com/tiangolo/typer/pull/549) by [@pre-commit-ci[bot]](https://github.com/apps/pre-commit-ci).
* 🔧 Add `exclude_lines` to coverage configuration. PR [#585](https://github.com/tiangolo/typer/pull/585) by [@dmontagu](https://github.com/dmontagu).
* ⬆️ Upgrade analytics. PR [#557](https://github.com/tiangolo/typer/pull/557) by [@tiangolo](https://github.com/tiangolo).
* 🔧 Update new issue chooser to suggest GitHub Discussions. PR [#544](https://github.com/tiangolo/typer/pull/544) by [@tiangolo](https://github.com/tiangolo).
* 🔧 Add GitHub Discussion templates for questions. PR [#541](https://github.com/tiangolo/typer/pull/541) by [@tiangolo](https://github.com/tiangolo).
* 🔧 Update pre-commit, Python version, isort version. PR [#542](https://github.com/tiangolo/typer/pull/542) by [@tiangolo](https://github.com/tiangolo).
* ⬆ [pre-commit.ci] pre-commit autoupdate. PR [#512](https://github.com/tiangolo/typer/pull/512) by [@pre-commit-ci[bot]](https://github.com/apps/pre-commit-ci).
* ⬆ Bump nwtgck/actions-netlify from 1.2.4 to 2.0.0. PR [#513](https://github.com/tiangolo/typer/pull/513) by [@dependabot[bot]](https://github.com/apps/dependabot).
* 👷 Refactor CI artifact upload/download for docs previews. PR [#516](https://github.com/tiangolo/typer/pull/516) by [@tiangolo](https://github.com/tiangolo).
* ⬆ [pre-commit.ci] pre-commit autoupdate. PR [#500](https://github.com/tiangolo/typer/pull/500) by [@pre-commit-ci[bot]](https://github.com/apps/pre-commit-ci).
* ⬆ Bump actions/cache from 2 to 3. PR [#496](https://github.com/tiangolo/typer/pull/496) by [@dependabot[bot]](https://github.com/apps/dependabot).
* ⬆ Bump dawidd6/action-download-artifact from 2.24.1 to 2.24.2. PR [#494](https://github.com/tiangolo/typer/pull/494) by [@dependabot[bot]](https://github.com/apps/dependabot).
* ⬆ Bump dawidd6/action-download-artifact from 2.9.0 to 2.24.1. PR [#491](https://github.com/tiangolo/typer/pull/491) by [@dependabot[bot]](https://github.com/apps/dependabot).
* ⬆ Bump actions/setup-python from 2 to 4. PR [#492](https://github.com/tiangolo/typer/pull/492) by [@dependabot[bot]](https://github.com/apps/dependabot).
* 👷‍♂️ Consistently use `sys.executable` to run subprocesses, needed by OpenSUSE. PR [#408](https://github.com/tiangolo/typer/pull/408) by [@theMarix](https://github.com/theMarix).
* 👷‍♂️ Ensure the `PYTHONPATH` is set properly when testing the tutorial scripts. PR [#407](https://github.com/tiangolo/typer/pull/407) by [@theMarix](https://github.com/theMarix).

## 0.7.0

### Features

* ✨ Make `typer.run()` not add completion scripts by default, it only makes sense in installed apps. Also update docs for handling [autocompletion in CLI options](https://typer.tiangolo.com/tutorial/options-autocompletion/). PR [#488](https://github.com/tiangolo/typer/pull/488) by [@tiangolo](https://github.com/tiangolo).
* ✨ Add support for Python 3.11, tests in CI and official marker. PR [#487](https://github.com/tiangolo/typer/pull/487) by [@tiangolo](https://github.com/tiangolo).
* 👷 Add CI for Python 3.10. PR [#384](https://github.com/tiangolo/typer/pull/384) by [@tiangolo](https://github.com/tiangolo).

### Fixes

* 🎨 Fix type annotation of `typer.run()`. PR [#284](https://github.com/tiangolo/typer/pull/284) by [@yassu](https://github.com/yassu).
* 🎨 Fix type annotations for `get_group`. PR [#430](https://github.com/tiangolo/typer/pull/430) by [@tiangolo](https://github.com/tiangolo).

### Docs

* 📝 Add note about how subcommands with function names using underscores are converted to dashes. PR [#403](https://github.com/tiangolo/typer/pull/403) by [@targhs](https://github.com/targhs).
* 📝 Fix typo in docs at `docs/tutorial/commands/help.md`. PR [#466](https://github.com/tiangolo/typer/pull/466) by [@fepegar](https://github.com/fepegar).
* ✏ Fix link in docs to `datetime.strptime()`. PR [#464](https://github.com/tiangolo/typer/pull/464) by [@Kobu](https://github.com/Kobu).
* ✏ Update `first-steps.md`, clarify distinction between parameter and argument. PR [#176](https://github.com/tiangolo/typer/pull/176) by [@mccarthysean](https://github.com/mccarthysean).
* ✏ Fix broken plac link. PR [#275](https://github.com/tiangolo/typer/pull/275) by [@mgielda](https://github.com/mgielda).

### Internal

* ✅ Add extra tests just for coverage because monkeypatching with strange imports confuses coverage. PR [#490](https://github.com/tiangolo/typer/pull/490) by [@tiangolo](https://github.com/tiangolo).
* 🔧 Tweak pytest coverage. PR [#485](https://github.com/tiangolo/typer/pull/485) by [@tiangolo](https://github.com/tiangolo).
* ➕ Bring back pytest-cov because coverage can't detect pytest-xdist. PR [#484](https://github.com/tiangolo/typer/pull/484) by [@tiangolo](https://github.com/tiangolo).
* ⬆ Bump actions/upload-artifact from 2 to 3. PR [#477](https://github.com/tiangolo/typer/pull/477) by [@dependabot[bot]](https://github.com/apps/dependabot).
* ⬆ Bump actions/checkout from 2 to 3. PR [#478](https://github.com/tiangolo/typer/pull/478) by [@dependabot[bot]](https://github.com/apps/dependabot).
* ⬆ [pre-commit.ci] pre-commit autoupdate. PR [#411](https://github.com/tiangolo/typer/pull/411) by [@pre-commit-ci[bot]](https://github.com/apps/pre-commit-ci).
* ⬆ Bump nwtgck/actions-netlify from 1.1.5 to 1.2.4. PR [#479](https://github.com/tiangolo/typer/pull/479) by [@dependabot[bot]](https://github.com/apps/dependabot).
* ⬆ Bump tiangolo/issue-manager from 0.2.0 to 0.4.0. PR [#481](https://github.com/tiangolo/typer/pull/481) by [@dependabot[bot]](https://github.com/apps/dependabot).
* 👷 Move from pytest-cov to coverage and Codecov to Smokeshow. PR [#483](https://github.com/tiangolo/typer/pull/483) by [@tiangolo](https://github.com/tiangolo).
* ➕ Add extra Material for MkDocs deps for docs. PR [#482](https://github.com/tiangolo/typer/pull/482) by [@tiangolo](https://github.com/tiangolo).
* 🔧 Update Dependabot config. PR [#476](https://github.com/tiangolo/typer/pull/476) by [@tiangolo](https://github.com/tiangolo).

## 0.6.1

### Fixes

* 🐛 Fix setting `FORCE_TERMINAL` with colors 2. PR [#424](https://github.com/tiangolo/typer/pull/424) by [@tiangolo](https://github.com/tiangolo).
* 🐛 Fix setting `FORCE_TERMINAL` with colors. PR [#423](https://github.com/tiangolo/typer/pull/423) by [@tiangolo](https://github.com/tiangolo).

## 0.6.0

This release adds deep integrations with [Rich](https://rich.readthedocs.io/en/stable/). ✨

`rich` is an optional dependency, you can install it directly or it will be included when you install with:

```console
$ pip install "typer[all]"
```

If Rich is available, it will be used to show the content from `--help` options, validation errors, and even errors in your app (exception tracebacks).

There are new options to group commands, *CLI arguments*, and *CLI options*, support for [Rich Console Markup](https://rich.readthedocs.io/en/stable/markup.html), and more! 🎉

### Features

* ✨ Richify, add integrations with Rich everywhere. PR [#419](https://github.com/tiangolo/typer/pull/419) by [@tiangolo](https://github.com/tiangolo).
    * Recommend Rich as the main information displaying tool, new docs: [Printing and Colors](https://typer.tiangolo.com/tutorial/printing/).
    * For most use cases not using Rich, use plain `print()` instead of `typer.echo()` in the docs, to simplify the concepts and avoid confusions. New docs: [Printing and Colors - typer Echo](https://typer.tiangolo.com/tutorial/printing/#typer-echo).
    * Define help panels for *CLI arguments*, new docs: [CLI Arguments with Help - CLI Argument help panels](https://typer.tiangolo.com/tutorial/arguments/help/#cli-argument-help-panels).
    * Define help panels for *CLI options*, new docs: [CLI Options with Help - CLI Options help panels](https://typer.tiangolo.com/tutorial/options/help/#cli-options-help-panels).
    * New docs for deprecating commands: [Commands - Command Help - Deprecate a Command](https://typer.tiangolo.com/tutorial/commands/help/#deprecate-a-command).
    * Support for Rich Markdown in docstrings, *CLI parameters* `help`, and `epilog` with the new parameter `typer.Typer(rich_markup_mode="markdown")`, new docs: [Commands - Command Help - Rich Markdown and Markup](https://typer.tiangolo.com/tutorial/commands/help/#rich-markdown-and-markup).
    * Support for Rich Markup (different from Markdown) in docstrings, *CLI parameters* `help`, and `epilog` with the new parameter `typer.Typer(rich_markup_mode="rich")`, new docs: [Commands - Command Help - Rich Markdown and Markup](https://typer.tiangolo.com/tutorial/commands/help/#rich-markdown-and-markup).
    * Define help panels for *commands*, new docs: [Commands - Command Help - Help Panels](https://typer.tiangolo.com/tutorial/commands/help/#help-panels).
    * New docs for setting an `epilog`, with support for Rich Markdown and Console Markup, new docs: [Commands - Command Help - Epilog](https://typer.tiangolo.com/tutorial/commands/help/#epilog).
* ✨ Refactor and document handling pretty exceptions. PR [#422](https://github.com/tiangolo/typer/pull/422) by [@tiangolo](https://github.com/tiangolo).
    * Add support for customizing pretty short errors, new docs: [Exceptions and Errors](https://typer.tiangolo.com/tutorial/exceptions/).
* ✨ Allow configuring pretty errors when creating the Typer instance. PR [#416](https://github.com/tiangolo/typer/pull/416) by [@tiangolo](https://github.com/tiangolo).

### Docs

* 📝 Add docs for using Rich with Typer. PR [#421](https://github.com/tiangolo/typer/pull/421) by [@tiangolo](https://github.com/tiangolo).
    * Add new docs: [Ask with Prompt - Prompt with Rich](https://typer.tiangolo.com/tutorial/prompt/#prompt-with-rich).
    * Add new docs to handle progress bars and spinners with Rich: [Progress Par](https://typer.tiangolo.com/tutorial/progressbar/).

### Internal

* ⬆️ Upgrade codecov GitHub Action. PR [#420](https://github.com/tiangolo/typer/pull/420) by [@tiangolo](https://github.com/tiangolo).

## 0.5.0

### Features

* ✨ Add pretty error tracebacks for user errors and support for Rich. PR [#412](https://github.com/tiangolo/typer/pull/412) by [@tiangolo](https://github.com/tiangolo).

### Docs

* ✏ Fix typo, "ASCII codes" to "ANSI escape sequences". PR [#308](https://github.com/tiangolo/typer/pull/308) by [@septatrix](https://github.com/septatrix).

## 0.4.2

### Fixes

* 🐛 Fix type conversion for `List` and `Tuple` and their internal types. PR [#143](https://github.com/tiangolo/typer/pull/143) by [@hellowhistler](https://github.com/hellowhistler).
* 🐛 Fix `context_settings` for a Typer app with a single command. PR [#210](https://github.com/tiangolo/typer/pull/210) by [@daddycocoaman](https://github.com/daddycocoaman).

### Docs

* 📝 Clarify testing documentation about checking `stderr`. PR [#335](https://github.com/tiangolo/typer/pull/335) by [@cgabard](https://github.com/cgabard).
* ✏ Fix typo in docs for CLI Option autocompletion. PR [#288](https://github.com/tiangolo/typer/pull/288) by [@graue70](https://github.com/graue70).
* 🎨 Fix header format for "Standard Input" in `docs/tutorial/printing.md`. PR [#386](https://github.com/tiangolo/typer/pull/386) by [@briancohan](https://github.com/briancohan).
* ✏ Fix typo in `docs/tutorial/terminating.md`. PR [#382](https://github.com/tiangolo/typer/pull/382) by [@kianmeng](https://github.com/kianmeng).
* ✏ Fix syntax typo in `docs/tutorial/package.md`. PR [#333](https://github.com/tiangolo/typer/pull/333) by [@ryanstreur](https://github.com/ryanstreur).
* ✏ Fix typo, duplicated word in `docs/tutorial/options/required.md`.. PR [#316](https://github.com/tiangolo/typer/pull/316) by [@michaelriri](https://github.com/michaelriri).
* ✏ Fix minor typo in `index.md`. PR [#274](https://github.com/tiangolo/typer/pull/274) by [@RmStorm](https://github.com/RmStorm).
* ✏ Fix double "and" typo in first-steps tutorial. PR [#225](https://github.com/tiangolo/typer/pull/225) by [@softwarebloat](https://github.com/softwarebloat).
* 🎨 Fix format in docs explaining `datetime` parameter type. PR [#220](https://github.com/tiangolo/typer/pull/220) by [@DiegoPiloni](https://github.com/DiegoPiloni).

### Internal

* ⬆ [pre-commit.ci] pre-commit autoupdate. PR [#404](https://github.com/tiangolo/typer/pull/404) by [@pre-commit-ci[bot]](https://github.com/apps/pre-commit-ci).
* 👷 Fix Material for MkDocs install in CI. PR [#395](https://github.com/tiangolo/typer/pull/395) by [@tiangolo](https://github.com/tiangolo).
* 👷 Add pre-commit CI config. PR [#394](https://github.com/tiangolo/typer/pull/394) by [@tiangolo](https://github.com/tiangolo).
* 👷 Clear MkDocs Insiders cache. PR [#393](https://github.com/tiangolo/typer/pull/393) by [@tiangolo](https://github.com/tiangolo).
* 🔧 Add pre-commit config and formatting. PR [#392](https://github.com/tiangolo/typer/pull/392) by [@tiangolo](https://github.com/tiangolo).
* 👷 Disable installing MkDocs Insiders in forks. PR [#391](https://github.com/tiangolo/typer/pull/391) by [@tiangolo](https://github.com/tiangolo).
* ⬆️ Upgrade Codecov GitHub Action. PR [#383](https://github.com/tiangolo/typer/pull/383) by [@tiangolo](https://github.com/tiangolo).

## 0.4.1

### Fixes

* 🐛 Fix import of `get_terminal_size` for Click 8.1.0 support and upgrade Black to fix CI. PR [#380](https://github.com/tiangolo/typer/pull/380) by [@tiangolo](https://github.com/tiangolo) based on original PR [#375](https://github.com/tiangolo/typer/pull/375) by [@madkinsz](https://github.com/madkinsz).

### Internal

* 📝 Add Jina's QA Bot to the docs to help people that want to ask quick questions. PR [#368](https://github.com/tiangolo/typer/pull/368) by [@tiangolo](https://github.com/tiangolo).
* 💚 Only test on push when on master, avoid duplicate CI runs from PRs. PR [#358](https://github.com/tiangolo/typer/pull/358) by [@tiangolo](https://github.com/tiangolo).
* ✨ Add support for previewing docs in PRs from forks and enable MkDocs Insiders. PR [#357](https://github.com/tiangolo/typer/pull/357) by [@tiangolo](https://github.com/tiangolo).
* ⬆️ Upgrade MkDocs Material, MDX-Include, and MkDocs structure. PR [#356](https://github.com/tiangolo/typer/pull/356) by [@tiangolo](https://github.com/tiangolo).
* 👷 Update publish GitHub action. PR [#325](https://github.com/tiangolo/typer/pull/325) by [@tiangolo](https://github.com/tiangolo).

## 0.4.0

### Features

* ✨ Add support for Click 8 while keeping compatibility with Click 7. PR [#317](https://github.com/tiangolo/typer/pull/317) by [@tiangolo](https://github.com/tiangolo).

### Internal

* 📝 Add Security policy. PR [#324](https://github.com/tiangolo/typer/pull/324) by [@tiangolo](https://github.com/tiangolo).
* 🔧 Add updated issue templates. PR [#323](https://github.com/tiangolo/typer/pull/323) by [@tiangolo](https://github.com/tiangolo).
* 👷 Enable tests for Python 3.9. PR [#322](https://github.com/tiangolo/typer/pull/322) by [@tiangolo](https://github.com/tiangolo).
* 👷 Add GitHub Action Latest Changes. PR [#321](https://github.com/tiangolo/typer/pull/321) by [@tiangolo](https://github.com/tiangolo).
* 👷 Update docs CI name. PR [#320](https://github.com/tiangolo/typer/pull/320) by [@tiangolo](https://github.com/tiangolo).
* 🔧 Add sponsors docs and badge. PR [#319](https://github.com/tiangolo/typer/pull/319) by [@tiangolo](https://github.com/tiangolo).

## 0.3.2

### Features

* Add support for `mypy --strict`. Original PR [#147](https://github.com/tiangolo/typer/pull/147) by [@victorphoenix3](https://github.com/victorphoenix3).

### Docs

* Update docs with new `--help` showing default values. PR [#135](https://github.com/tiangolo/typer/pull/135) by [@victorphoenix3](https://github.com/victorphoenix3).
* Add `Optional` to docs for *CLI Arguments and Options* with a default of `None`. PR [#131](https://github.com/tiangolo/typer/pull/131) by [@rkbeatss](https://github.com/rkbeatss).
* Add valid date formats to docs. PR [#122](https://github.com/tiangolo/typer/pull/122) by [@IamCathal](https://github.com/IamCathal).

### Internal

* Report coverage in XML to support GitHub Actions. PR [#146](https://github.com/tiangolo/typer/pull/146).
* Update badges and remove Travis, now that GitHub Actions is the main CI. PR [#145](https://github.com/tiangolo/typer/pull/145).

## 0.3.1

* Add GitHub Actions, move from Travis. PR [#144](https://github.com/tiangolo/typer/pull/144).
* Pin dependencies. PR [#138](https://github.com/tiangolo/typer/pull/138).
* Add Dependabot. PR [#136](https://github.com/tiangolo/typer/pull/136).
* Upgrade Isort to version 5.x.x. PR [#137](https://github.com/tiangolo/typer/pull/137).

## 0.3.0

* Add support for `help` parameter in *CLI arguments*:
    * As `help` in *CLI arguments* is not supported by Click, there are two new internal classes (Click sub-classes) to support it:
        * `typer.core.TyperArgument`
        * `typer.core.TyperCommand`
    * This includes a new auto-generated help text section `Arguments` for *CLI arguments*, showing defaults, required arguments, etc.
    * It's also possible to disable it and keep the previous behavior, not showing automatic help for *CLI arguments* (Click's default) using the `hidden` parameter.
    * Now `show_default` is `True` by default.
    * And now `show_envvar` is `True` by default.
    * So, default values and env vars are shown in the help text by default, without having to manually enable them, for both *CLI arguments* and *CLI options*.
    * New docs:
        * [CLI Arguments Intro](https://typer.tiangolo.com/tutorial/arguments/).
        * [Optional CLI Arguments](https://typer.tiangolo.com/tutorial/arguments/optional/).
        * [CLI Arguments with Default](https://typer.tiangolo.com/tutorial/arguments/default/).
        * [CLI Arguments with Help](https://typer.tiangolo.com/tutorial/arguments/help/).
        * [CLI Arguments with Environment Variables](https://typer.tiangolo.com/tutorial/arguments/envvar/).
        * [CLI Arguments: Other uses](https://typer.tiangolo.com/tutorial/arguments/other-uses/).
        * [CLI arguments with tuples](https://typer.tiangolo.com/tutorial/multiple-values/arguments-with-multiple-values/#cli-arguments-with-tuples).
    * Lot's of tests for all the new examples in the new docs, keeping coverage at 100%.
    * PR [#123](https://github.com/tiangolo/typer/pull/123).
* Add docs for calling packages with `python -m some_package` using `__main__.py`: [Building a Package: Support `python -m`](https://typer.tiangolo.com/tutorial/package/#support-python-m-optional). PR [#121](https://github.com/tiangolo/typer/pull/121).
* Add support for `*args` and `**kwargs` when calling the Typer app, just like in Click. PR [#120](https://github.com/tiangolo/typer/pull/120) by [@teymour-aldridge](https://github.com/teymour-aldridge).
* Fix typos in README and main docs [#103](https://github.com/tiangolo/typer/pull/103) by [@mrcartoonster](https://github.com/mrcartoonster).
* Fix typo in docs. PR [#98](https://github.com/tiangolo/typer/pull/98) by [@mrcartoonster](https://github.com/mrcartoonster).
* Fix typos and rewording in docs. PR [#97](https://github.com/tiangolo/typer/pull/97) by [@mrcartoonster](https://github.com/mrcartoonster).
* Update GitHub Action issue-manager. PR [#114](https://github.com/tiangolo/typer/pull/114).

## 0.2.1

* Add support for forward references (types declared inside of strings). PR [#93](https://github.com/tiangolo/typer/pull/93).

## 0.2.0

* Add support for completion for commands/programs not available on startup.
    * This allows installing a Typer program/script in a virtual environment and still have completion globally installed.
    * PR [#92](https://github.com/tiangolo/typer/pull/92).
* Add note about `typer.echo()` and `print()` for colors in Windows. PR [#89](https://github.com/tiangolo/typer/pull/89).
* Upgrade Mkdocs-Material version, update contributing guide style. PR [#90](https://github.com/tiangolo/typer/pull/90).

## 0.1.1

* Fix completion evaluation for Bash and Zsh when the program is not installed/found. PR [#83](https://github.com/tiangolo/typer/pull/83).
* Fix completion script for Fish. PR [#82](https://github.com/tiangolo/typer/pull/82).
* Fix shell installation for Bash to `~/.bashrc` and update Windows development docs. PR [#81](https://github.com/tiangolo/typer/pull/81).
* Update coverage badge. PR [#78](https://github.com/tiangolo/typer/pull/78).

## 0.1.0

* Fix coverage instructions. PR [#72](https://github.com/tiangolo/typer/pull/72).
* Add docs for [Building a Package](https://typer.tiangolo.com/tutorial/package/). PR [#71](https://github.com/tiangolo/typer/pull/71).
* Add docs for [Using Click (with Typer)](https://typer.tiangolo.com/tutorial/using-click/). PR [#70](https://github.com/tiangolo/typer/pull/70).
* Add support for type-based callbacks and autocompletion functions, extra tests and docs:
    * Extra tests, raising coverage to 100%.
    * New docs: [Printing and Colors: "Standard Output" and "Standard Error"](https://typer.tiangolo.com/tutorial/printing/#standard-output-and-standard-error).
    * New docs: [Password CLI Option and Confirmation Prompt](https://typer.tiangolo.com/tutorial/options/password/).
    * Support for callbacks based on type annotations. New docs: [CLI Option Callback and Context](https://typer.tiangolo.com/tutorial/options/callback-and-context/).
    * New docs: [Version CLI Option, is_eager](https://typer.tiangolo.com/tutorial/options/version/).
    * Support for autocompletion functions based on type annotations. New docs: [CLI Option autocompletion](https://typer.tiangolo.com/tutorial/options/autocompletion/).
    * New docs: [Commands: Using the Context](https://typer.tiangolo.com/tutorial/commands/context/).
    * New docs: [Testing](https://typer.tiangolo.com/tutorial/testing/).
    * PR [#68](https://github.com/tiangolo/typer/pull/68).
* Fix Zsh completion install script. PR [#69](https://github.com/tiangolo/typer/pull/69).
* Fix typo in progressbar example. PR [#63](https://github.com/tiangolo/typer/pull/63) by [@ValentinCalomme](https://github.com/ValentinCalomme).

## 0.0.11

* Re-implement completion system:
    * Remove optional dependency `click-completion` (with its sub-dependencies, like Jinja).
    * Add optional dependency `shellingham` to auto detect shell to install (it was used by `click-completion`).
    * Completion now doesn't require a third party library.
        * If `shellingham` is not installed/added as a dependency, `--install-completion` and `--show-completion` take a value with the name of the shell.
    * Fix support for user provided completion in *CLI Parameters*.
    * Fix completion for files in Bash, Zsh, and Fish.
    * Add support for modern versions of PowerShell, 5, 6, and 7 (e.g. in Windows 10).
    * Add support for `pwsh` (PowerShell Core).
        * PowerShell support includes help strings for commands and *CLI Parameters*.
    * Several bug fixes.
    * Tests for the completion logic/code.
    * Tested in all the shells in Linux and Windows.
    * PR [#66](https://github.com/tiangolo/typer/pull/66).
* Fix format in docs with highlighted lines. PR [#65](https://github.com/tiangolo/typer/pull/65).
* Add docs about [Typer CLI - completion for small scripts](https://typer.tiangolo.com/typer-cli/). PR [#64](https://github.com/tiangolo/typer/pull/64).
* Add docs about [Alternatives, Inspiration and Comparisons](https://typer.tiangolo.com/alternatives/). PR [#62](https://github.com/tiangolo/typer/pull/62).
* Add [Development - Contributing Guide](https://typer.tiangolo.com/contributing/). PR [#61](https://github.com/tiangolo/typer/pull/61).

## 0.0.10

* Add support for Click version 7.1.1. PR [#60](https://github.com/tiangolo/typer/pull/60).

## 0.0.9

* Add support for PEP 561, to allow `mypy` to type check applications built with **Typer**. PR [#58](https://github.com/tiangolo/typer/pull/58).
* Upgrade deploy docs to Netlify GitHub action. PR [#57](https://github.com/tiangolo/typer/pull/57).
* Add support for Mermaid JS for visualizations. PR [#56](https://github.com/tiangolo/typer/pull/56).
* Update CI to run docs deployment in GitHub actions. PR [#50](https://github.com/tiangolo/typer/pull/50).
* Update format for internal links. PR [#38](https://github.com/tiangolo/typer/pull/38).
* Tweak external links' format. PR [#36](https://github.com/tiangolo/typer/pull/36).

## 0.0.8

* Update docs and add latest changes to MkDocs/website. PR [#33](https://github.com/tiangolo/typer/pull/33).
* Add extra tests for edge cases that don't belong in docs' examples. PR [#32](https://github.com/tiangolo/typer/pull/32).
* Add docs for CLI Parameters with [Multiple Values](https://typer.tiangolo.com/tutorial/multiple-values/). Includes tests for all the examples and bug fixes. PR [#31](https://github.com/tiangolo/typer/pull/31).
* Add docs for extra *CLI parameter* types: [CLI Parameter Types: Number](https://typer.tiangolo.com/tutorial/parameter-types/number/) and [CLI Parameter Types: Boolean CLI Options](https://typer.tiangolo.com/tutorial/parameter-types/bool/). PR [#30](https://github.com/tiangolo/typer/pull/30).
* Extend docs for Commands, add [Commands: Typer Callback](https://typer.tiangolo.com/tutorial/commands/callback/) and [Commands: One or Multiple](https://typer.tiangolo.com/tutorial/commands/one-or-multiple/). This includes tests for all the examples and bug fixes. PR [#29](https://github.com/tiangolo/typer/pull/29).
* Add docs for [SubCommands - Command Groups](https://typer.tiangolo.com/tutorial/subcommands/). This includes tests for all the examples and bug fixes. PR [#28](https://github.com/tiangolo/typer/pull/28).
* Remove unneeded code for argument handling. PR [#26](https://github.com/tiangolo/typer/pull/26).
* Add docs for [Launching Applications](https://typer.tiangolo.com/tutorial/launch/). PR [#25](https://github.com/tiangolo/typer/pull/25).
* Add docs for getting the [CLI Application Directory](https://typer.tiangolo.com/tutorial/app-dir/). PR [#24](https://github.com/tiangolo/typer/pull/24).
* Add docs for [Progress Bars](https://typer.tiangolo.com/tutorial/progressbar/). PR [#23](https://github.com/tiangolo/typer/pull/23).
* Add docs for [Asking with Interactive Prompts](). PR [#22](https://github.com/tiangolo/typer/pull/22).
* Update docs for path *CLI option*. PR [#21](https://github.com/tiangolo/typer/pull/21).
* Add colors module and docs for [Printing and Colors](https://typer.tiangolo.com/tutorial/printing/) and for [Terminating](https://typer.tiangolo.com/tutorial/terminating/), including tests. PR [#20](https://github.com/tiangolo/typer/pull/20).
* Refactor docs to make each individual page/section "bite-sized" / small. Add docs for [CLI option names](https://typer.tiangolo.com/tutorial/options/name/). Update `typer.Argument()` to remove invalid positional `param_decls`. PR [#19](https://github.com/tiangolo/typer/pull/19).

## 0.0.7

* Add docs for [*CLI parameter* types](https://typer.tiangolo.com/tutorial/parameter-types/). Includes tests and file classes refactor. PR [#17](https://github.com/tiangolo/typer/pull/17).
* Add tests for completion. PR [#15](https://github.com/tiangolo/typer/pull/15) and [#16](https://github.com/tiangolo/typer/pull/16).

## 0.0.6

* Add docs for [Commands](https://typer.tiangolo.com/tutorial/commands/). Includes a bug fix for handling default values set in `typer.Typer()` parameters. PR [#14](https://github.com/tiangolo/typer/pull/14).
* Add docs for [CLI Arguments](https://typer.tiangolo.com/tutorial/arguments/). PR [#13](https://github.com/tiangolo/typer/pull/13).
* Add docs for [CLI Options](https://typer.tiangolo.com/tutorial/options/). PR [#12](https://github.com/tiangolo/typer/pull/12).

## 0.0.5

* Clean exports from Typer. Remove unneeded components from Click and add needed `Exit` exception. PR [#11](https://github.com/tiangolo/typer/pull/11).
* Fix and document extracting help from a function's docstring [First Steps: Document your CLI app](https://typer.tiangolo.com/tutorial/first-steps/#document-your-cli-app). PR [#10](https://github.com/tiangolo/typer/pull/10).
* Update references to `--install-completion` and `--show-completion` in docs. PR [#9](https://github.com/tiangolo/typer/pull/9).
* Fix testing utilities, add tests for First Steps examples. PR [#8](https://github.com/tiangolo/typer/pull/8).
* Add auto completion options by default when [click-completion](https://github.com/click-contrib/click-completion) is installed: `--install-completion` and `--show-completion`. PR [#7](https://github.com/tiangolo/typer/pull/7).
* Update Termynal to have fixed sizes, add "fast" button, and use it in [First Steps](https://typer.tiangolo.com/tutorial/first-steps/). PR [#6](https://github.com/tiangolo/typer/pull/6).
* Add custom automatic [Termynal](https://github.com/tiangolo/termynal) for docs. PR [#5](https://github.com/tiangolo/typer/pull/5).

## 0.0.4

* Update short descriptions and assets.
* Docs rewording and fix typos. PR [#1](https://github.com/tiangolo/typer/pull/1) by [@mariacamilagl](https://github.com/mariacamilagl).

## 0.0.3

* Fix group creation without name.

## 0.0.2

* Add initial version of code, docs, etc.

## 0.0.1

* First commit. Publish to PyPI to reserve package name.
