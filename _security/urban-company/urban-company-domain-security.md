---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: urbancompany.com
  spf: true
hosts:
- cert_expires: Oct  7 01:38:49 2026 GMT
  host: www.urbancompany.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Urban Company Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Urban Company, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Urban Company
provider_slug: urban-company
slug: urban-company-domain-security
source_filename: urban-company-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.urbancompany.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 01:38:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: urbancompany.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/urban-company/refs/heads/main/security/urban-company-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Home Services
- Marketplace
- Beauty
- Appliance Repair
- Cleaning
- On-Demand
---
