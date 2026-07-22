---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: resourcewise.com
  spf: true
hosts:
- cert_expires: Sep 21 01:38:13 2026 GMT
  host: www.resourcewise.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Resourcewise Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ResourceWise, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ResourceWise
provider_slug: resourcewise
slug: resourcewise-domain-security
source_filename: resourcewise-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.resourcewise.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 01:38:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: resourcewise.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/resourcewise/refs/heads/main/security/resourcewise-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Market Intelligence
- Commodities
- Data and Analytics
- Forest Products
- Pulp and Paper
- Chemicals
- Biofuels
- Pricing Data
- Sustainability
---
