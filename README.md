# dbtproj

This is a dbt project that is designed to work with a dagster project in another Git repository.

The GitHub action has been adapted to dispatch an action on `https://github.com/slopp/dagsterproj` which then clones this project into the dagster project and deploys to Dagster Cloud. PRs to this repository will create a Dagster Cloud branch deployment, but comments will not be added to the PR in this repo.