---
api_specs:
- filename: scrapybara-openapi.yml
  format: yaml
  label: Scrapybara Instances API
  slug: scrapybara-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scrapybara/refs/heads/main/openapi/scrapybara-openapi.yml
- filename: scrapybara-openapi.yml
  format: yaml
  label: Scrapybara Computer Actions API
  slug: scrapybara-computer-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scrapybara/refs/heads/main/openapi/scrapybara-openapi.yml
- filename: scrapybara-openapi.yml
  format: yaml
  label: Scrapybara Browser API
  slug: scrapybara-browser-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scrapybara/refs/heads/main/openapi/scrapybara-openapi.yml
- filename: scrapybara-openapi.yml
  format: yaml
  label: Scrapybara Code Execution API
  slug: scrapybara-code-execution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scrapybara/refs/heads/main/openapi/scrapybara-openapi.yml
- filename: scrapybara-openapi.yml
  format: yaml
  label: Scrapybara Filesystem API
  slug: scrapybara-filesystem-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scrapybara/refs/heads/main/openapi/scrapybara-openapi.yml
- filename: scrapybara-openapi.yml
  format: yaml
  label: Scrapybara Notebook API
  slug: scrapybara-notebook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scrapybara/refs/heads/main/openapi/scrapybara-openapi.yml
- filename: scrapybara-openapi.yml
  format: yaml
  label: Scrapybara Auth States API
  slug: scrapybara-auth-states-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scrapybara/refs/heads/main/openapi/scrapybara-openapi.yml
- filename: scrapybara-openapi.yml
  format: yaml
  label: Scrapybara Environment API
  slug: scrapybara-environment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scrapybara/refs/heads/main/openapi/scrapybara-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: scrapybara.com
  spf: false
hosts:
- cert_expires: Sep 30 10:42:13 2026 GMT
  host: scrapybara.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 05:40:43 2026 GMT
  host: docs.scrapybara.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 19 18:03:25 2026 GMT
  host: api.scrapybara.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Scrapybara Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Scrapybara, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Scrapybara
provider_slug: scrapybara
slug: scrapybara-domain-security
source_filename: scrapybara-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: scrapybara.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 10:42:13 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.scrapybara.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 05:40:43 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.scrapybara.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 18:03:25 2026 GMT\n  hsts: null\ndomains:\n- domain: scrapybara.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scrapybara/refs/heads/main/security/scrapybara-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI Agents
- Virtual Desktops
- Computer Use
- Browser Automation
- Code Execution
---
