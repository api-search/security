---
api_key_in: []
api_specs:
- filename: selenium-cookies-api-openapi.yml
  format: yaml
  label: Selenium Cookies API
  slug: selenium-cookies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/selenium/refs/heads/main/openapi/selenium-cookies-api-openapi.yml
- filename: selenium-elements-api-openapi.yml
  format: yaml
  label: Selenium Elements API
  slug: selenium-elements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/selenium/refs/heads/main/openapi/selenium-elements-api-openapi.yml
- filename: selenium-navigation-api-openapi.yml
  format: yaml
  label: Selenium Navigation API
  slug: selenium-navigation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/selenium/refs/heads/main/openapi/selenium-navigation-api-openapi.yml
- filename: selenium-script-api-openapi.yml
  format: yaml
  label: Selenium Script API
  slug: selenium-script-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/selenium/refs/heads/main/openapi/selenium-script-api-openapi.yml
- filename: selenium-session-api-openapi.yml
  format: yaml
  label: Selenium Session API
  slug: selenium-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/selenium/refs/heads/main/openapi/selenium-session-api-openapi.yml
- filename: selenium-status-api-openapi.yml
  format: yaml
  label: Selenium Status API
  slug: selenium-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/selenium/refs/heads/main/openapi/selenium-status-api-openapi.yml
auth_types: []
description: 'Authentication model for the Selenium WebDriver wire protocol and Selenium Grid. The W3C WebDriver standard defines NO authentication — that is a deliberate property of the standard, not an omission by Selenium. Security is a deployment concern: run the remote end on a private network, front it with a reverse proxy, or turn on Grid''s built-in HTTP Basic. derive-authentication.py produced no profile for this provider precisely because the captured OpenAPI declares no securitySchemes; everything below is read from the Grid documentation instead.'
kind: authentication
layout: security
method: searched
name: Selenium Authentication
name_suffix: Authentication
oauth_flows: []
overview: Selenium declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Selenium
provider_slug: selenium
scheme_count: 3
schemes:
- applies_to: WebDriver remote end (chromedriver, geckodriver, msedgedriver, safaridriver, standalone)
  description: No authentication. Any process that can reach the port can create a session and drive a browser, execute arbitrary JavaScript in it, and read its cookies.
  evidence: 'openapi/_original/selenium-openapi.yml info.description: "No authentication is defined by the W3C protocol itself; deployments typically front the endpoint with a reverse proxy or run on a private network."'
  id: none
  type: none
- applies_to: Selenium Grid server (Standalone, Hub, Router)
  configuration:
  - description: User name clients must use to connect to the server.
    example: admin
    flag: --username
    type: string
  - description: Password clients must use to connect to the server.
    example: myStrongPassword
    flag: --password
    type: string
  description: HTTP Basic authentication on the Grid server, enabled by setting BOTH --username and --password. The docs are explicit that neither works alone.
  docs: https://www.selenium.dev/documentation/grid/configuration/cli_options/
  id: basic
  required_together: true
  scheme: basic
  type: http
- applies_to: Node registration and Distributor administrative endpoints
  configuration:
  - description: Shared secret used to authenticate Node registration requests. Must match the value set on the Hub/Distributor.
    example: '"Hunter2"'
    flag: --registration-secret
    type: string
  description: A shared secret authenticating Node registration requests to the Hub/Distributor, and required on the Grid administrative endpoints. Configured with --registration-secret and it must match on both ends.
  docs: https://www.selenium.dev/documentation/grid/advanced_features/endpoints/
  empty_secret_form: If no registration secret has been configured, the header is still required but sent empty — the documented form is `--header 'X-REGISTRATION-SECRET;'` (note the trailing semicolon, curl's empty-header syntax). An agent that omits the header entirely gets a different failure than one that sends it empty.
  id: registration-secret
  in: header
  name: X-REGISTRATION-SECRET
  type: apiKey
  usage_example: 'curl --request DELETE ''http://localhost:4444/se/grid/distributor/node/<node-id>'' --header ''X-REGISTRATION-SECRET: <secret>'''
slug: selenium-authentication
source_filename: selenium-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: >-\n  https://www.selenium.dev/documentation/grid/configuration/cli_options/ (Server and Node sections,\n  read 2026-08-26), https://www.selenium.dev/documentation/grid/advanced_features/endpoints/,\n  https://www.w3.org/TR/webdriver2/, and openapi/_original/selenium-openapi.yml\nprovider: Selenium\nproviderId: selenium\ndescription: >-\n  Authentication model for the Selenium WebDriver wire protocol and Selenium Grid. The W3C WebDriver\n  standard defines NO authentication — that is a deliberate property of the standard, not an\n  omission by Selenium. Security is a deployment concern: run the remote end on a private network,\n  front it with a reverse proxy, or turn on Grid's built-in HTTP Basic. derive-authentication.py\n  produced no profile for this provider precisely because the captured OpenAPI declares no\n  securitySchemes; everything below is read from the Grid documentation instead.\nschemes:\n  - id: none\n    type:\
  \ none\n    applies_to: WebDriver remote end (chromedriver, geckodriver, msedgedriver, safaridriver, standalone)\n    description: >-\n      No authentication. Any process that can reach the port can create a session and drive a\n      browser, execute arbitrary JavaScript in it, and read its cookies.\n    evidence: >-\n      openapi/_original/selenium-openapi.yml info.description: \"No authentication is defined by the\n      W3C protocol itself; deployments typically front the endpoint with a reverse proxy or run on a\n      private network.\"\n  - id: basic\n    type: http\n    scheme: basic\n    applies_to: Selenium Grid server (Standalone, Hub, Router)\n    description: >-\n      HTTP Basic authentication on the Grid server, enabled by setting BOTH --username and\n      --password. The docs are explicit that neither works alone.\n    configuration:\n      - flag: --username\n        type: string\n        example: admin\n        description: User name clients must use to connect to\
  \ the server.\n      - flag: --password\n        type: string\n        example: myStrongPassword\n        description: Password clients must use to connect to the server.\n    required_together: true\n    docs: https://www.selenium.dev/documentation/grid/configuration/cli_options/\n  - id: registration-secret\n    type: apiKey\n    in: header\n    name: X-REGISTRATION-SECRET\n    applies_to: Node registration and Distributor administrative endpoints\n    description: >-\n      A shared secret authenticating Node registration requests to the Hub/Distributor, and required\n      on the Grid administrative endpoints. Configured with --registration-secret and it must match\n      on both ends.\n    configuration:\n      - flag: --registration-secret\n        type: string\n        example: '\"Hunter2\"'\n        description: >-\n          Shared secret used to authenticate Node registration requests. Must match the value set on\n          the Hub/Distributor.\n    usage_example: >-\n      curl\
  \ --request DELETE 'http://localhost:4444/se/grid/distributor/node/<node-id>'\n      --header 'X-REGISTRATION-SECRET: <secret>'\n    empty_secret_form: >-\n      If no registration secret has been configured, the header is still required but sent empty —\n      the documented form is `--header 'X-REGISTRATION-SECRET;'` (note the trailing semicolon, curl's\n      empty-header syntax). An agent that omits the header entirely gets a different failure than one\n      that sends it empty.\n    docs: https://www.selenium.dev/documentation/grid/advanced_features/endpoints/\ntransport_security:\n  - flag: --https-certificate\n    type: path\n    description: Server certificate for HTTPS.\n  - flag: --https-private-key\n    type: path\n    description: Private key for HTTPS (PKCS8).\ntransport_security_note: >-\n  TLS is opt-in and off by default; the documented default base is plain http://localhost:4444.\n  `java -jar selenium-server.jar info security` prints the project's own security guidance.\n\
  network_exposure:\n  - flag: --allow-cors\n    default: false\n    description: >-\n      Whether the Selenium server should allow web-browser connections from any host. Leaving this\n      off is what keeps a page under test from driving the Grid that is testing it.\n  - flag: --bind-host\n    description: >-\n      Whether the server binds to the host address or only uses it to report its reachable URL.\n      Relevant when deciding what the remote end is actually listening on.\n  - flag: --sub-path\n    example: my_company/selenium_grid\n    description: A sub-path the server should serve from, e.g. when reverse-proxied.\noauth: false\noidc: false\nmtls: false\napi_keys: false\nguidance_for_agents: >-\n  Treat a WebDriver endpoint as an unauthenticated remote-code-execution surface unless you put auth\n  in front of it. POST /session/{sessionId}/execute/sync runs arbitrary JavaScript in a real browser\n  under the identity of whatever is loaded in it, and GET /session/{sessionId}/cookie\
  \ returns that\n  browsing context's cookies. Neither requires a credential by default. If you are exposing a Grid\n  beyond localhost, set --username/--password, set --registration-secret, and enable HTTPS.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/selenium/refs/heads/main/authentication/selenium-authentication.yml
summary_line: 3 schemes
tags:
- Automation
- Browsers
- End-to-End Testing
- Quality Assurance
- Testing
- WebDriver
---
