---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ambrook.com
  spf: true
hosts:
- cert_expires: Aug 28 08:38:06 2026 GMT
  host: ambrook.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ambrook Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ambrook, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Ambrook
provider_slug: ambrook
slug: ambrook-domain-security
source_filename: ambrook-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ambrook.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 08:38:06 2026 GMT\n  hsts: false\ndomains:\n- domain: ambrook.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ambrook/refs/heads/main/security/ambrook-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Fintech
- Agriculture
- Accounting
- Bookkeeping
- Payments
- Farm Management
- MCP
---
