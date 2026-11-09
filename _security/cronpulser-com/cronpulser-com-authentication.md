---
anonymous_access: false
api_key_in: []
api_specs:
- filename: cronpulser-com-openapi-generated.yml
  format: yaml
  label: CronPulser API
  slug: cronpulser-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cronpulser-com/openapi/_ae-authored/cronpulser-com-openapi-generated.yml
auth_types: []
description: Authentication methods for CronPulser APIs and MCP integration.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Cronpulser Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: CronPulser declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: CronPulser
provider_slug: cronpulser-com
scheme_count: 2
schemes:
- evidence: Your client discovers CronPulser’s OAuth endpoints automatically. Sign in to CronPulser in the browser and review the requested scopes. Approve the connection. The client receives short-lived access and a rotating refresh token.
  flows:
  - client_credentials
  - authorization_code
  how_to_obtain: Sign in to CronPulser via the browser consent screen; the client receives an access token and refresh token.
  name: CronPulser MCP OAuth
  scopes:
  - list_projects
  - read
  - create_project
  - update_project
  - delete_project
  - list_jobs
  - get_job
  - list_execution_logs
  - get_job_stats
  - create_http_job
  - create_runner_job
  - create_tls_job
  - update_job
  - delete_job
  - pause_job
  - resume_job
  - trigger_job
  - list_alerts
  - get_alert
  - create_alert
  - update_alert
  - set_alert_active
  - resolve_alert
  - delete_alert
  - list_alert_history
  - list_runners
  - get_runner
  - create_runner
  type: oauth2
- evidence: 'Use a Bearer API key Administrators create keys from API Keys . The full cp_live_ value is displayed once. Send it in every request: Authorization: Bearer cp_live_your_key'
  header: Authorization
  how_to_obtain: Create an API key in the CronPulser UI under API Keys; the key is shown once.
  name: API Key
  type: http-bearer
slug: cronpulser-com-authentication
source_filename: cronpulser-com-authentication.yml
source_heading: Authentication Profile
source_url: https://cronpulser.com/docs/mcp/
source_yaml: "generated: '2026-11-04'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://cronpulser.com/docs/mcp/\nsources:\n- https://cronpulser.com/docs/mcp/\n- https://cronpulser.com/docs/api/\n- https://cronpulser.com/docs/runner/\n- https://cronpulser.com/docs/runner/\ndescription: Authentication methods for CronPulser APIs and MCP integration.\nschemes:\n- type: oauth2\n  name: CronPulser MCP OAuth\n  evidence: Your client discovers CronPulser’s OAuth endpoints automatically. Sign in to CronPulser in the browser and review the requested scopes.\n    Approve the connection. The client receives short-lived access and a rotating refresh token.\n  flows:\n  - client_credentials\n  - authorization_code\n  scopes:\n  - list_projects\n  - read\n  - create_project\n  - update_project\n  - delete_project\n  - list_jobs\n  - get_job\n  - list_execution_logs\n  - get_job_stats\n  - create_http_job\n  - create_runner_job\n  - create_tls_job\n  - update_job\n  - delete_job\n\
  \  - pause_job\n  - resume_job\n  - trigger_job\n  - list_alerts\n  - get_alert\n  - create_alert\n  - update_alert\n  - set_alert_active\n  - resolve_alert\n  - delete_alert\n  - list_alert_history\n  - list_runners\n  - get_runner\n  - create_runner\n  how_to_obtain: Sign in to CronPulser via the browser consent screen; the client receives an access token and refresh token.\n- type: http-bearer\n  name: API Key\n  evidence: 'Use a Bearer API key Administrators create keys from API Keys . The full cp_live_ value is displayed once. Send it in every request:\n    Authorization: Bearer cp_live_your_key'\n  header: Authorization\n  how_to_obtain: Create an API key in the CronPulser UI under API Keys; the key is shown once.\ndocs: https://cronpulser.com/docs/mcp/\n"
source_yaml_url: https://artifacts.apis.io/cronpulser-com/authentication/cronpulser-com-authentication.yml
summary_line: 2 schemes
tags:
- HTTP Scheduler
- API Scheduling
- runner
- TLS Monitoring
---
