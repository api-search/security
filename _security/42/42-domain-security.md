---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: 42technologies.com
  spf: true
hosts:
- cert_expires: Oct  4 19:29:07 2026 GMT
  host: 42technologies.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: 42 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 42 Technologies, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: 42 Technologies
provider_slug: '42'
slug: 42-domain-security
source_filename: 42-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 42technologies.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 19:29:07 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: 42technologies.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/42/refs/heads/main/security/42-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Retail
- Business Intelligence
- Analytics
- Reporting
- Ecommerce
- Omnichannel
- Retail Analytics
- Data
- Dashboards
---
