---
api_specs:
- filename: doit-openapi-original.yml
  format: yaml
  label: DoiT API
  slug: doit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doit/refs/heads/main/openapi/doit-openapi-original.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: doit.com
  spf: true
hosts:
- cert_expires: Oct 14 19:01:37 2026 GMT
  host: www.doit.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  1 05:34:13 2026 GMT
  host: developer.doit.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 14 19:01:37 2026 GMT
  host: api.doit.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Doit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DoiT, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: DoiT
provider_slug: doit
slug: doit-domain-security
source_filename: doit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.doit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 19:01:37 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: developer.doit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 05:34:13 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.doit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 19:01:37 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: doit.com\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/doit/refs/heads/main/security/doit-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- FinOps
- Cloud Cost Management
- Cloud Intelligence
- Cost Optimization
- Multicloud
- Kubernetes
- Analytics
- MCP
- Artificial Intelligence
---
