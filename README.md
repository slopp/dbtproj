# dbtproj

This is a dbt project that is designed to work with a dagster project in another Git repository.

The GitHub action has been adapted to dispatch an action on `https://github.com/slopp/dagsterproj` which then clones this project into the dagster project and deploys to Dagster Cloud. PRs to this repository will also create a Dagster Cloud branch deployment.

In order for these actions to work, you will need to create a GitHub Actions secret for this repository called `PAT_TOKEN` thas has access to read/write to both the dbt project repository and the dagster project. Additionally, you will want to modify the script inside the action to refer to your dagster project's repository.