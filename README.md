# gh-projects-field-ids v1

![workflow badge](https://github.com/infinite-automations/gh-projects-field-ids/actions/workflows/test.yml/badge.svg)

Gets the id of a github project custom field or a select option. 

# Usage

```yaml
- uses: infinite-automations/gh-projects-field-ids@v1
  with:
    # token which is used to access the project data via GitHub CLI
    token: ''
    # number of the project. Value is integer and can be found in the url of the project view. Example url: https://github.com/orgs/infinite-automations/projects/1/settings
    project-number: ''
    # Name of the field to get the id from.
    # Camel Case is important!
    field-name: ''
    # Name of the selection option to get the id from.
    # Camel Case is important!
    select-option-name: ''
```

# Outputs

| Output Name | Description                     | 
| ----------- | ------------------------------- |
| field-id    | id for the field with the name equals ```field-name``` |
| select-option-id | id for the select option with the name equals ```select-option-name``` |

# License

The scripts and documentation in this project are released under the MIT License.