# GitHub Repository Manager

Thank you for installing the official GitHub Repository Manager application!

This application provides a suite of flows to help you manage your GitHub repositories directly from the `cx` shell.

---

## Required Connections

During installation, you were prompted to set up a connection with the logical ID `github_api`. This is the connection all flows in this application will use.

## Available Flows

### `list-issues`

Fetches open issues for a specific repository.

**Usage:**

```
cx> flow run list-issues owner=<repository-owner> repo=<repository-name>
```

**Example:**

```
cx> flow run list-issues owner=facebook repo=react --output table --query "'List Repository Issues'.[].{number:number, title:title, user:user.login}"
```

---

_(More flows will be added in future versions!)_
