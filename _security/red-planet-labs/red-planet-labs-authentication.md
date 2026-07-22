---
api_key_in: []
auth_types:
- none
description: Authentication profile for Rama's built-in REST API. Rama is deployed by the user onto their own cluster; the REST API documentation describes no application-layer authentication scheme (no API key, token, OAuth, or mTLS). Access is expected to be governed at the network/deployment boundary of the self-hosted cluster rather than by the API itself.
kind: authentication
layout: security
method: searched
name: Red Planet Labs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Red Planet Labs secures its APIs with none across 0 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Red Planet Labs
provider_slug: red-planet-labs
scheme_count: 0
schemes: []
slug: red-planet-labs-authentication
source_filename: red-planet-labs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://redplanetlabs.com/docs/~/rest.html\ndescription: >-\n  Authentication profile for Rama's built-in REST API. Rama is deployed by the\n  user onto their own cluster; the REST API documentation describes no\n  application-layer authentication scheme (no API key, token, OAuth, or mTLS).\n  Access is expected to be governed at the network/deployment boundary of the\n  self-hosted cluster rather than by the API itself.\nsummary:\n  types:\n  - none\nschemes: []\nnotes: >-\n  Because Rama is self-hosted software rather than a public cloud API, there is no\n  vendor-issued credential. Operators are responsible for network isolation,\n  firewalling, and any reverse-proxy authentication placed in front of Supervisor\n  daemons and the Conductor UI (default port 8888).\ndocs: https://redplanetlabs.com/docs/~/rest.html\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/red-planet-labs/refs/heads/main/authentication/red-planet-labs-authentication.yml
summary_line: none · 0 schemes
tags:
- Company
- Enterprise Saas
- Backend Platform
- Distributed Systems
- Database
- JVM
- Clojure
- Java
- Developer Tools
- Rama
---
