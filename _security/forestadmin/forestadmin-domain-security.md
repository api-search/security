---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Forest Admin REST API (Admin Backend)
  slug: admin-api
  spec_type: OpenAPI
  url: https://forestadmin.github.io/agent-nodejs/
description: ''
domains:
- caa:
  - 128 issue "letsencrypt.org"
  - 128 issue "pki.goog"
  - 128 issue "amazon.com"
  - 128 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: forestadmin.com
  spf: true
hosts:
- cert_expires: Dec 30 23:59:59 2026 GMT
  host: www.forestadmin.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 29 23:59:59 2026 GMT
  host: docs.forestadmin.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 18 23:59:59 2026 GMT
  host: app.forestadmin.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Forestadmin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Forest Admin, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Forest Admin
provider_slug: forestadmin
slug: forestadmin-domain-security
source_filename: forestadmin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.forestadmin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.forestadmin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.forestadmin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: forestadmin.com\n  dnssec: false\n  caa:\n  - 128 issue \"letsencrypt.org\"\n  - 128 issue \"pki.goog\"\n  - 128 issue \"amazon.com\"\n  - 128 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/forestadmin/refs/heads/main/security/forestadmin-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- admin panel
- internal tools
- RBAC
- workflow automation
- CRUD
- operations
- fintech
- compliance
- low-code
- AI agents
---
