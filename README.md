# FLECS Create Repository Variable Action
A GitHub action to create repository variables

# Usage
## Example
```yml
uses: FLECS-Technologies/create-repository-variable-action@v1.x
with:
  repo: "repository-name"
  owner: "organization"
  name: "MY_VARIABLE"
  value: "my_variable_value"
env:
  GITHUB_TOKEN: "access token with with variables repo permission"
```

# Inputs
| Name          | Description             | Example              | Required | Default |
| ------------- | ------------------------| -------------------- | -------- | ------- |
| repo          | Name of the repository  | "awesome-project"    | Yes      | -       |
| owner         | Repository owner        | "FLECS-Technologies" | Yes      | -       |
| name          | Name of the variable    | "MY_VARIABLE"        | Yes      | -       |
| value         | Value of the variable   | "my_variable_value"  | Yes      | -       |

See [GitHub REST API documentation]([https://docs.github.com/en/rest/actions/variables?apiVersion=2022-11-28#create-a-repository-variable) for further examples and explanation.

# Environment
| Name          | Description                                                                                                  | Required |
| ------------- | ------------------------------------------------------------------------------------------------------------ | ---------|
| GITHUB\_TOKEN | A GitHub access token or GitHub Apps installastion token with the "Variables" repository permissions (write) | true     |

# License
[Apache 2.0](https://github.com/FLECS-Technologies/add-collaborator-action/blob/v1.x/LICENSE)
