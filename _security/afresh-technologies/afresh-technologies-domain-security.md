---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: afresh.com
  spf: true
hosts:
- cert_expires: Oct  8 02:43:15 2026 GMT
  host: www.afresh.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Afresh Technologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Afresh Technologies, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Afresh Technologies
provider_slug: afresh-technologies
slug: afresh-technologies-domain-security
source_filename: afresh-technologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.afresh.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 02:43:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: afresh.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/afresh-technologies/refs/heads/main/security/afresh-technologies-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Grocery
- Retail
- Artificial Intelligence
- Supply Chain
- Inventory Management
- Demand Forecasting
- Food Waste
- Fresh Food
---
