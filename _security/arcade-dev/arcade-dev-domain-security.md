---
api_specs:
- filename: arcade-dev-admin-api-openapi.yml
  format: yaml
  label: arcade-dev Admin API
  slug: arcade-dev-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcade-dev/refs/heads/main/openapi/arcade-dev-admin-api-openapi.yml
- filename: arcade-dev-authorization-api-openapi.yml
  format: yaml
  label: arcade-dev Authorization API
  slug: arcade-dev-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcade-dev/refs/heads/main/openapi/arcade-dev-authorization-api-openapi.yml
- filename: arcade-dev-gateways-api-openapi.yml
  format: yaml
  label: arcade-dev Gateways API
  slug: arcade-dev-gateways-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcade-dev/refs/heads/main/openapi/arcade-dev-gateways-api-openapi.yml
- filename: arcade-dev-hooks-api-openapi.yml
  format: yaml
  label: arcade-dev Hooks API
  slug: arcade-dev-hooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcade-dev/refs/heads/main/openapi/arcade-dev-hooks-api-openapi.yml
- filename: arcade-dev-llm-api-openapi.yml
  format: yaml
  label: arcade-dev LLM API
  slug: arcade-dev-llm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcade-dev/refs/heads/main/openapi/arcade-dev-llm-api-openapi.yml
- filename: arcade-dev-operations-api-openapi.yml
  format: yaml
  label: arcade-dev Operations API
  slug: arcade-dev-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcade-dev/refs/heads/main/openapi/arcade-dev-operations-api-openapi.yml
- filename: arcade-dev-plugins-api-openapi.yml
  format: yaml
  label: arcade-dev Plugins API
  slug: arcade-dev-plugins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcade-dev/refs/heads/main/openapi/arcade-dev-plugins-api-openapi.yml
- filename: arcade-dev-tools-api-openapi.yml
  format: yaml
  label: arcade-dev Tools API
  slug: arcade-dev-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcade-dev/refs/heads/main/openapi/arcade-dev-tools-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: arcade.dev
  spf: true
hosts:
- cert_expires: Oct  2 20:45:23 2026 GMT
  host: arcade.dev
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 23:21:23 2026 GMT
  host: docs.arcade.dev
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 13 17:58:19 2026 GMT
  host: api.arcade.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Arcade Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Arcade.dev, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Arcade.dev
provider_slug: arcade-dev
slug: arcade-dev-domain-security
source_filename: arcade-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: arcade.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 20:45:23 2026 GMT\n  hsts: true\n  hsts_max_age: 0\n- host: docs.arcade.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 23:21:23 2026 GMT\n  hsts: true\n  hsts_max_age: 0\n- host: api.arcade.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 17:58:19 2026 GMT\n  hsts: null\ndomains:\n- domain: arcade.dev\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arcade-dev/refs/heads/main/security/arcade-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags: []
---
