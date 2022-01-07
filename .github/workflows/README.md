# Workflows

## Reusable workflows
Workflows which may be called by any repository (both within and outside of TV4 organisation).
[Learn about reusable workflows.](https://docs.github.com/en/actions/learn-github-actions/reusing-workflows)

### terraform.yml
- Handles `terraform` lifecycle.
- `terraform apply` is only performed on a designated `live-branch` (input parameter, defaults to `main`). 
- Creates comments in PRs with highlighted `terraform plan` outputs.
- Current supported providers: [Google Provider](https://registry.terraform.io/providers/hashicorp/google/latest/docs/guides/getting_started).

**Used by following repositories:**
  1. https://github.com/TV4/data-airflow-dags
  2. https://github.com/TV4/data-bigquery 
