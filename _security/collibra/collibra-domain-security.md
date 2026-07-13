---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: collibra.com
  spf: true
hosts:
- cert_expires: Sep 14 15:28:25 2026 GMT
  host: www.collibra.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 18:03:10 2026 GMT
  host: developer.collibra.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Collibra Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Collibra, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Collibra
provider_slug: collibra
slug: collibra-domain-security
source_filename: collibra-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.collibra.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 15:28:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.collibra.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 18:03:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: collibra.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/collibra/refs/heads/main/security/collibra-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Data Governance
- Data Management
- Data Catalog
- Data Quality
- AI Governance
- Data Lineage
- Enterprise Software
---
