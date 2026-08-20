---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: barclaycardus.com
  spf: true
hosts:
- cert_expires: Dec  4 23:59:59 2026 GMT
  host: cards.barclaycardus.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Barclays Us Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Barclays US, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Barclays US
provider_slug: barclays-us
slug: barclays-us-domain-security
source_filename: barclays-us-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cards.barclaycardus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: barclaycardus.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/barclays-us/refs/heads/main/security/barclays-us-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial-Services
- Banking
- United States
- Credit Cards
- Consumer Banking
- Co-Brand Cards
- Open Finance
- Data Aggregation
---
