---
api_specs:
- filename: railway-app-asyncapi.yml
  format: yaml
  label: Railway Logs API
  slug: railway-app-logs-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/railway-app/refs/heads/main/asyncapi/railway-app-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: railway.com
  spf: true
hosts:
- cert_expires: Sep 14 09:27:50 2026 GMT
  host: railway.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  2 17:08:08 2026 GMT
  host: docs.railway.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 23:19:47 2026 GMT
  host: backboard.railway.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Railway App Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Railway, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Railway
provider_slug: railway-app
slug: railway-app-domain-security
source_filename: railway-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: railway.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 09:27:50 2026 GMT\n  hsts: false\n- host: docs.railway.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 17:08:08 2026 GMT\n  hsts: false\n- host: backboard.railway.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 23:19:47 2026 GMT\n  hsts: false\ndomains:\n- domain: railway.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/railway-app/refs/heads/main/security/railway-app-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Deployment
- PaaS
- Cloud
- Infrastructure
- GraphQL
- DevOps
---
