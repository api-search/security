---
api_key_in:
- header
api_specs:
- filename: shoppable-cloud-openapi-original.yml
  format: yaml
  label: Shoppable Commerce API Suite
  slug: shoppable-commerce-api-suite
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shoppable/refs/heads/main/openapi/shoppable-cloud-openapi-original.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Shoppable Authentication
name_suffix: Authentication
oauth_flows: []
overview: Shoppable secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Shoppable
provider_slug: shoppable
scheme_count: 2
schemes:
- description: 'Token provided by your Customer Success Manager


    **For Internal Endpoints (/internal/*):**

    ```

    Kolu72V3T3eFplHNe66e8aef90aba018

    ```


    **For Regular API Endpoints (default test customer):**

    ```

    U2FsdGVkX192JseAYpgNqMvh5tRQJwAfc4xoA5PKFiXbgWqH2FGD4obxczwL4EEgrj4jVCDxrAblAy3b2W/SK1R3jCWtwQ1fyqQvhfdZGUoXktXwz0tpYfi0I7bVsvQil4D1TeqirpzX66lZ467EFDogCwlWBkoEuhFZNHNnYoQW2LT3Mr5GMIdfBgIcvx6QrtE24Q5pnIBzBDY4'
  name: Bearer
  scheme: bearer
  sources:
  - openapi/shoppable-cloud-openapi-original.yml
  type: http
- description: 'Authorization header provided by your Customer Success Manager


    **For Internal Endpoints (/internal/*):**

    ```

    40ba20012ddf314e43234ee53b4b20f2

    ```


    **For Regular API Endpoints:**

    ```

    test_secret_12345678901234567890

    ```'
  in: header
  name: Secret
  parameter: x-shoppable-secret
  sources:
  - openapi/shoppable-cloud-openapi-original.yml
  type: apiKey
slug: shoppable-authentication
source_filename: shoppable-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/shoppable-cloud-openapi-original.yml\ndocs: https://about.shoppable.com/help/setup-developer-documentation\nmodel: >-\n  Dual-header auth. Every request must send both Authorization: Bearer <token>\n  and x-shoppable-secret: <secret>. Both credentials are issued by your\n  Shoppable Customer Success Manager. No OAuth / OpenID Connect.\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: Bearer\n  type: http\n  scheme: bearer\n  description: |-\n    Token provided by your Customer Success Manager\n\n    **For Internal Endpoints (/internal/*):**\n    ```\n    Kolu72V3T3eFplHNe66e8aef90aba018\n    ```\n\n    **For Regular API Endpoints (default test customer):**\n    ```\n    U2FsdGVkX192JseAYpgNqMvh5tRQJwAfc4xoA5PKFiXbgWqH2FGD4obxczwL4EEgrj4jVCDxrAblAy3b2W/SK1R3jCWtwQ1fyqQvhfdZGUoXktXwz0tpYfi0I7bVsvQil4D1TeqirpzX66lZ467EFDogCwlWBkoEuhFZNHNnYoQW2LT3Mr5GMIdfBgIcvx6QrtE24Q5pnIBzBDY4\n \
  \ sources:\n  - openapi/shoppable-cloud-openapi-original.yml\n- name: Secret\n  type: apiKey\n  in: header\n  parameter: x-shoppable-secret\n  description: |-\n    Authorization header provided by your Customer Success Manager\n\n    **For Internal Endpoints (/internal/*):**\n    ```\n    40ba20012ddf314e43234ee53b4b20f2\n    ```\n\n    **For Regular API Endpoints:**\n    ```\n    test_secret_12345678901234567890\n    ```\n  sources:\n  - openapi/shoppable-cloud-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shoppable/refs/heads/main/authentication/shoppable-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Commerce
- E-Commerce
- Checkout
- Catalog
- Payments
- Agentic Commerce
- MCP
- Embeddable Commerce
- Retail
---
