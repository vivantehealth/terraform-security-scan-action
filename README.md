# terraform-security-scan-action

Suggested use:

```yaml
jobs:
  security-scan:
    name: Security scan
    runs-on: ubuntu-latest
    defaults:
      run:
        working-directory: ${{ env.tf_actions_working_dir }}
    steps:
      - name: Terraform Security Scan
        uses: vivantehealth/terraform-security-scan-action@main
        with:
          github_token: ${{ secrets.GITHUB_TOKEN }}
```
