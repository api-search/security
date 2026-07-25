---
api_specs:
- filename: shortcut-categories-api-openapi.yml
  format: yaml
  label: Shortcut Categories API
  slug: shortcut-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shortcut/refs/heads/main/openapi/shortcut-categories-api-openapi.yml
- filename: shortcut-custom-fields-api-openapi.yml
  format: yaml
  label: Shortcut Custom Fields API
  slug: shortcut-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shortcut/refs/heads/main/openapi/shortcut-custom-fields-api-openapi.yml
- filename: shortcut-documents-api-openapi.yml
  format: yaml
  label: Shortcut Documents API
  slug: shortcut-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shortcut/refs/heads/main/openapi/shortcut-documents-api-openapi.yml
- filename: shortcut-entity-templates-api-openapi.yml
  format: yaml
  label: Shortcut Entity Templates API
  slug: shortcut-entity-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shortcut/refs/heads/main/openapi/shortcut-entity-templates-api-openapi.yml
- filename: shortcut-epics-api-openapi.yml
  format: yaml
  label: Shortcut Epics API
  slug: shortcut-epics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shortcut/refs/heads/main/openapi/shortcut-epics-api-openapi.yml
- filename: shortcut-workflows-api-openapi.yml
  format: yaml
  label: Shortcut Workflows API
  slug: shortcut-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shortcut/refs/heads/main/openapi/shortcut-workflows-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: shortcut.com
  spf: true
hosts:
- cert_expires: Jan 19 23:59:59 2027 GMT
  host: www.shortcut.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 23:59:59 2026 GMT
  host: developer.shortcut.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 27 23:59:59 2026 GMT
  host: api.app.shortcut.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Shortcut Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Shortcut, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Shortcut
provider_slug: shortcut
slug: shortcut-domain-security
source_filename: shortcut-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.shortcut.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 23:59:59 2027 GMT\n  hsts: false\n- host: developer.shortcut.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.app.shortcut.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: shortcut.com\n  dnssec: true\n  caa:\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shortcut/refs/heads/main/security/shortcut-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Project Management
- Agile
- Software Development
- Issue Tracking
- Kanban
- Sprint Planning
- Collaboration
- Developer Tools
---
