---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: planhat.com
  spf: true
hosts:
- cert_expires: Sep 22 14:17:32 2026 GMT
  host: www.planhat.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 04:28:08 2026 GMT
  host: api.planhat.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 17:02:50 2026 GMT
  host: analytics.planhat.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Planhat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Planhat, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Planhat
provider_slug: planhat
slug: planhat-domain-security
source_filename: planhat-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.planhat.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 14:17:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.planhat.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 04:28:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: analytics.planhat.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 17:02:50 2026 GMT\n  hsts: false\ndomains:\n- domain: planhat.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/planhat/refs/heads/main/security/planhat-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Saas
- Customer Success
- Customer Platform
- CRM
- Customer Data
- Analytics
- Revenue
- MCP
---
