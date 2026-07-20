---
description: ''
domains:
- caa:
  - 0 issue "amazonaws.com"
  - 0 issue "awstrust.com"
  - 0 issue "amazontrust.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: healthex.io
  spf: true
hosts:
- cert_expires: Aug 27 14:06:23 2026 GMT
  host: www.healthex.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 23:59:59 2026 GMT
  host: docs.healthex.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 31 23:59:59 2026 GMT
  host: api.healthex.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Healthex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HealthEx, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: HealthEx
provider_slug: healthex
slug: healthex-domain-security
source_filename: healthex-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.healthex.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 14:06:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.healthex.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.healthex.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: healthex.io\n  dnssec: true\n  caa:\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/healthex/refs/heads/main/security/healthex-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Healthcare
- Health Records
- FHIR
- Patient Consent
- Data Sharing
- Interoperability
- TEFCA
- MCP
- Agents
---
