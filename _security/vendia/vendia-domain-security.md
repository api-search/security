---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: vendia.com
  spf: true
hosts:
- cert_expires: Sep 15 13:25:46 2026 GMT
  host: www.vendia.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 09:23:44 2026 GMT
  host: docs.vendia.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 18 23:59:59 2027 GMT
  host: api.share.vendia.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vendia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vendia, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Vendia
provider_slug: vendia
slug: vendia-domain-security
source_filename: vendia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vendia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 13:25:46 2026 GMT\n  hsts: false\n- host: docs.vendia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 09:23:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.share.vendia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 18 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: vendia.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vendia/refs/heads/main/security/vendia-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- MCP
- Artificial Intelligence
- Data Sharing
- Data Platform
- GraphQL
- Agents
- API Gateway
- Data Governance
---
