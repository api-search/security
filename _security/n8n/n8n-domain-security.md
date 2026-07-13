---
api_specs:
- filename: n8n-openapi.yml
  format: yaml
  label: N8n
  slug: n8n
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/n8n/refs/heads/main/openapi/n8n-openapi.yml
- filename: n8n-openapi.yml
  format: yaml
  label: N8n REST API
  slug: n8n-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/n8n/refs/heads/main/openapi/n8n-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:security@n8n.io"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: n8n.io
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: n8n.cloud
  spf: true
hosts:
- cert_expires: Oct  3 02:40:24 2026 GMT
  host: n8n.io
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 11:12:10 2026 GMT
  host: docs.n8n.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 17 21:16:03 2026 GMT
  host: app.n8n.cloud
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: N8N Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for N8n, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: N8n
provider_slug: n8n
slug: n8n-domain-security
source_filename: n8n-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: n8n.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 02:40:24 2026 GMT\n  hsts: true\n  hsts_max_age: 0\n- host: docs.n8n.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 11:12:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.n8n.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 21:16:03 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: n8n.io\n  dnssec: true\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:security@n8n.io\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: n8n.cloud\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/n8n/refs/heads/main/security/n8n-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Agents
- Artificial Intelligence
- Integrations
---
