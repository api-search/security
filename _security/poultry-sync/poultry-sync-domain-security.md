---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: poultrysync.com
  spf: true
hosts:
- cert_expires: Sep 29 05:12:34 2026 GMT
  host: poultrysync.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Poultry Sync Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Poultry sync, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Poultry sync
provider_slug: poultry-sync
slug: poultry-sync-domain-security
source_filename: poultry-sync-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: poultrysync.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 05:12:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: poultrysync.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/poultry-sync/refs/heads/main/security/poultry-sync-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Agriculture
- Poultry
- Data Management
- Artificial Intelligence
- ERP Integration
- Food Supply Chain
---
