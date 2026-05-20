# GH Auto-Answer Bot

A reusable GitHub Action for auto-responding to issues and pull requests.

## Usage

```yaml
- name: Run Auto-Responder
  uses: jmaxdev/automatic-answer@v1
  with:
    token: ${{ secrets.GITHUB_TOKEN }}
    personal_token: ${{ secrets.PERSONAL_ACCESS_TOKEN || '' }}
    use_personal_token: ${{ secrets.PERSONAL_ACCESS_TOKEN != '' }}
    issue_comment: "Thank you for creating this issue! Our team will review it soon."
    pr_comment: "Thank you for your PR! We will review it shortly."
    add_labels: false
```

check the [action.yml](action.yml) for more 'with' fields.