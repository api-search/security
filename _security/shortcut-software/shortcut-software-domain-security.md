---
api_specs:
- filename: shortcut-software-openapi-original.json
  format: json
  label: Shortcut API
  slug: shortcut-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shortcut-software/refs/heads/main/openapi/shortcut-software-openapi-original.json
description: ''
domains:
- caa:
  - 0 iodef "mailto:ops@shortcut.com"
  - 0 issue ";"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: shortcut.com
  spf: true
hosts:
- cert_expires: Oct 27 23:59:59 2026 GMT
  host: api.app.shortcut.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Shortcut Software Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Shortcut Software, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Shortcut Software
provider_slug: shortcut-software
slug: shortcut-software-domain-security
source_filename: shortcut-software-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.app.shortcut.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: shortcut.com\n  dnssec: true\n  caa:\n  - 0 iodef \"mailto:ops@shortcut.com\"\n  - 0 issue \";\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shortcut-software/refs/heads/main/security/shortcut-software-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Project Management
- Issue Tracking
- Agile
- Developer Tools
- Software Development
- Sprints
- Roadmaps
---
