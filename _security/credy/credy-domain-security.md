---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: credy.com
  spf: true
hosts:
- cert_expires: Nov 14 18:13:47 2026 GMT
  host: www.credy.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Credy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Credy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Credy
provider_slug: credy
slug: credy-domain-security
source_filename: credy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.credy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 18:13:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: credy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/credy/refs/heads/main/security/credy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Advertising
- Finance
- AffiliateNetwork
- International
- Loans
---
