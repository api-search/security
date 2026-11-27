---
anonymous_access: false
api_key_in: []
api_specs:
- filename: sonarqube-issues-api-openapi.yml
  format: yaml
  label: SonarQube Issues API
  slug: sonarqube-issues-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sonarqube/openapi/sonarqube-issues-api-openapi.yml
- filename: sonarqube-measures-api-openapi.yml
  format: yaml
  label: SonarQube Measures API
  slug: sonarqube-measures-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sonarqube/openapi/sonarqube-measures-api-openapi.yml
- filename: sonarqube-projects-api-openapi.yml
  format: yaml
  label: SonarQube Projects API
  slug: sonarqube-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sonarqube/openapi/sonarqube-projects-api-openapi.yml
- filename: sonarqube-quality-gates-api-openapi.yml
  format: yaml
  label: SonarQube Quality Gates API
  slug: sonarqube-quality-gates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sonarqube/openapi/sonarqube-quality-gates-api-openapi.yml
- filename: sonarqube-rules-api-openapi.yml
  format: yaml
  label: SonarQube Rules API
  slug: sonarqube-rules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sonarqube/openapi/sonarqube-rules-api-openapi.yml
- filename: sonarqube-system-api-openapi.yml
  format: yaml
  label: SonarQube System API
  slug: sonarqube-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sonarqube/openapi/sonarqube-system-api-openapi.yml
- filename: sonarqube-users-api-openapi.yml
  format: yaml
  label: SonarQube Users API
  slug: sonarqube-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sonarqube/openapi/sonarqube-users-api-openapi.yml
auth_types:
- http
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: SonarQube Authentication
name_suffix: Authentication
oauth_flows: []
overview: SonarQube secures its APIs with http and apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: SonarQube
provider_slug: sonarqube
scheme_count: 3
schemes:
- description: HTTP basic authentication with the token as the username and an empty password ("pass the token using the bearer or basic HTTP authentication scheme").
  name: basicAuth
  scheme: basic
  sources:
  - openapi/sonarqube-issues-api-openapi.yml
  - openapi/sonarqube-measures-api-openapi.yml
  - openapi/sonarqube-projects-api-openapi.yml
  - openapi/sonarqube-quality-gates-api-openapi.yml
  - openapi/sonarqube-rules-api-openapi.yml
  - openapi/sonarqube-system-api-openapi.yml
  - openapi/sonarqube-users-api-openapi.yml
  type: http
- description: 'Bearer authentication with a SonarQube token: Authorization: Bearer <myToken>. Recommended scheme. Responses to token-authenticated calls carry a SonarQube-Authentication-Token-Expiration header with the token expiry date.'
  docs: https://docs.sonarsource.com/sonarqube-server/user-guide/managing-tokens/
  expiry: Optional expiration at creation (or No expiration unless an administrator enforces a maximum lifetime, Enterprise Edition and above); email reminder 7 days before expiry; expired tokens stop working but remain listed for revocation.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/sonarqube-issues-api-openapi.yml
  - openapi/sonarqube-measures-api-openapi.yml
  - openapi/sonarqube-projects-api-openapi.yml
  - openapi/sonarqube-quality-gates-api-openapi.yml
  - openapi/sonarqube-rules-api-openapi.yml
  - openapi/sonarqube-system-api-openapi.yml
  - openapi/sonarqube-users-api-openapi.yml
  token_types:
  - type: User
    use: any Web API action the user may perform in the UI; required for SonarQube for IDE connected mode and the SonarQube CLI
  - type: Project analysis
    use: run analyses on one project and call web services requiring Execute Analysis on it
  - type: Global analysis
    use: run analyses on every project
  type: http
- description: System passcode defined by sonar.web.systemPasscode in sonar.properties or the SONAR_WEB_SYSTEMPASSCODE environment variable; "If you cannot use the bearer authentication scheme (e.g., with the API endpoint monitoring/metrics), you can use the X-Sonar-Passcode authentication scheme."
  in: header
  name: systemPasscode
  parameter: X-Sonar-Passcode
  sources:
  - https://docs.sonarsource.com/sonarqube-server/extension-guide/web-api.md
  type: apiKey
slug: sonarqube-authentication
source_filename: sonarqube-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: searched\nsource:\n- https://docs.sonarsource.com/sonarqube-server/extension-guide/web-api.md\n- https://docs.sonarsource.com/sonarqube-server/user-guide/managing-tokens.md\n- https://docs.sonarsource.com/sonarqube-server/instance-administration/security/administering-tokens.md\n- openapi/sonarqube-issues-api-openapi.yml\n- openapi/sonarqube-measures-api-openapi.yml\n- openapi/sonarqube-projects-api-openapi.yml\n- openapi/sonarqube-quality-gates-api-openapi.yml\n- openapi/sonarqube-rules-api-openapi.yml\n- openapi/sonarqube-system-api-openapi.yml\n- openapi/sonarqube-users-api-openapi.yml\nsummary:\n  types:\n  - http\n  - apiKey\n  recommended: bearer\n  detail: '\"To authenticate to the Web API, we recommend that you use the bearer authentication scheme.\" Basic auth\n    with the token as username and an empty password is also accepted; the X-Sonar-Passcode header authenticates\n    monitoring endpoints such as api/monitoring/metrics with\
  \ the system passcode.'\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP basic authentication with the token as the username and an empty password (\"pass the token using\n    the bearer or basic HTTP authentication scheme\").\n  sources:\n  - openapi/sonarqube-issues-api-openapi.yml\n  - openapi/sonarqube-measures-api-openapi.yml\n  - openapi/sonarqube-projects-api-openapi.yml\n  - openapi/sonarqube-quality-gates-api-openapi.yml\n  - openapi/sonarqube-rules-api-openapi.yml\n  - openapi/sonarqube-system-api-openapi.yml\n  - openapi/sonarqube-users-api-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Bearer authentication with a SonarQube token: Authorization: Bearer <myToken>. Recommended scheme.\n    Responses to token-authenticated calls carry a SonarQube-Authentication-Token-Expiration header with the token\n    expiry date.'\n  sources:\n  - openapi/sonarqube-issues-api-openapi.yml\n  - openapi/sonarqube-measures-api-openapi.yml\n\
  \  - openapi/sonarqube-projects-api-openapi.yml\n  - openapi/sonarqube-quality-gates-api-openapi.yml\n  - openapi/sonarqube-rules-api-openapi.yml\n  - openapi/sonarqube-system-api-openapi.yml\n  - openapi/sonarqube-users-api-openapi.yml\n  token_types:\n  - type: User\n    use: any Web API action the user may perform in the UI; required for SonarQube for IDE connected mode and the\n      SonarQube CLI\n  - type: Project analysis\n    use: run analyses on one project and call web services requiring Execute Analysis on it\n  - type: Global analysis\n    use: run analyses on every project\n  expiry: Optional expiration at creation (or No expiration unless an administrator enforces a maximum lifetime,\n    Enterprise Edition and above); email reminder 7 days before expiry; expired tokens stop working but remain listed\n    for revocation.\n  docs: https://docs.sonarsource.com/sonarqube-server/user-guide/managing-tokens/\n- name: systemPasscode\n  type: apiKey\n  in: header\n  parameter: X-Sonar-Passcode\n\
  \  description: System passcode defined by sonar.web.systemPasscode in sonar.properties or the SONAR_WEB_SYSTEMPASSCODE\n    environment variable; \"If you cannot use the bearer authentication scheme (e.g., with the API endpoint monitoring/metrics),\n    you can use the X-Sonar-Passcode authentication scheme.\"\n  sources:\n  - https://docs.sonarsource.com/sonarqube-server/extension-guide/web-api.md\ndocs: https://docs.sonarsource.com/sonarqube-server/extension-guide/web-api/#authenticate-to-api\nnotes:\n- Administrative web services require specific permissions; a user token carries all permissions of its issuing\n  user.\n- OAuth is used only by the Sonar-hosted MCP service (mcp:tools:read / mcp:tools:write); the Web API itself has\n  no OAuth client flow. See mcp/sonarqube-mcp.yml.\n- Deactivating a user revokes all of that user's tokens.\n"
source_yaml_url: https://artifacts.apis.io/sonarqube/authentication/sonarqube-authentication.yml
summary_line: http/apiKey · 3 schemes
tags:
- Code Quality
- Developer Tools
- DevOps
- Security
- Static Analysis
- Code Security
- SAST
---
