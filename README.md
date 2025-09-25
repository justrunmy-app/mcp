# JustRunMy.App MCP Server

JustRunMy.App is a lightweight hosting platform built to remove the headaches of deployment. Instead of wrestling with servers, configs, or Docker, you can publish apps in seconds - from IDEs like Cursor or VS Code, or simply by uploading your code.  

We designed it for hobbyists, tinkerers, and indie builders who want to share their projects quickly and cheaply, without learning DevOps. With the new MCP server, your AI assistant can not only help you write code, but also deploy, manage, and update your apps directly.

This repository contains instructions on how to connect to the **JustRunMy.App MCP server** and start using it with your IDE or agent.

---

## 🔑 Access

1. Register at [https://justrunmy.app](https://justrunmy.app).
2. Sign in to your account.
3. In the left-side menu, open **MCP Server Config**.

---

## ⚡ Quick Setup with Cursor

Inside **MCP Server Config**, you will see a button:

**`Add to Cursor`**

- Click it, and the config will be automatically added to your Cursor IDE.  
- Restart Cursor if needed, then the MCP tools will appear in your IDE.

---

## ⚙️ Manual Setup (Other IDEs/Agents)

- Only **remote MCP server** is available.  
- There are **no local client transports** such as `stdio` or executables.  

To set up:

1. Copy the **Remote MCP Server Config** provided on the MCP Server Config page.
2. Paste it into your IDE/agent configuration where it expects MCP server entries.
3. Save & reload.

---

## Available MCP Tools

| Tool Name | Description |
|-----------|-------------|
| `jrnm_get_user_apps` | List all applications you have access to on JustRunMy.App. |
| `jrnm_get_app_status` | Get the current status and endpoints of a specific application. |
| `jrnm_get_app_logs` | Retrieve recent logs for an application to monitor and debug. |
| `jrnm_get_app_ports` | View port mappings for an application (internal ↔ external). |
| `jrnm_get_app_volumes` | List persistent storage volumes attached to an application. |
| `jrnm_get_env_vars` | Get all environment variables set for an application. |
| `jrnm_get_app_deploy_info_using_git` | Get a Git URL to push code and trigger deployment for an existing app. |
| `jrnm_get_new_app_deploy_info_using_git` | Get a Git URL to create and deploy a brand-new application. |
| `jrnm_add_app_volume` | Attach a new persistent storage volume to an application. |
| `jrnm_remove_app_volume` | Detach and delete a persistent volume from an application. |
| `jrnm_rename_app` | Change the display name of an application. |
| `jrnm_set_app_built_image` | Deploy a pre-built image to an application. |
| `jrnm_set_app_docker_image` | Deploy an image from a Docker registry to an application. |
| `jrnm_set_app_ports` | Define port mappings for an application. |
| `jrnm_set_app_quotas` | Set CPU and RAM limits for an application. |
| `jrnm_set_app_command` | Override the startup command for an application. |
| `jrnm_set_env_vars` | Replace all environment variables for an application. |
| `jrnm_update_env_var` | Add or update a single environment variable for an application. |
| `jrnm_start_or_restart_app` | Start or restart an application (apply new configs). |
| `jrnm_stop_app` | Stop a running application. |
| `jrnm_delete_app` | Permanently delete an application and its resources. |
| `jrnm_execute_command_in_app` | Run a shell command inside a running application container. |

---

## 📬 Support

For all support inquiries, please email: **support@justrunmy.app**
