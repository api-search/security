---
description: ''
domains:
- caa:
  - 0 issuewild "amazon.com;"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: infogram.com
  spf: true
hosts:
- cert_expires: Jan 22 23:59:59 2027 GMT
  host: infogram.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Infogram Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Infogram, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Infogram
provider_slug: infogram
slug: infogram-domain-security
source_filename: infogram-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: infogram.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 22 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: infogram.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazon.com;\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/infogram/refs/heads/main/security/infogram-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Data Visualization
- Infographics
- Charts
- Dashboards
- Reporting
- Business Intelligence
- Content
- Embeds
---
