---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: efex.com
  spf: true
hosts:
- cert_expires: Nov 25 23:59:59 2026 GMT
  host: efex.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Efex Ventu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EFEX (Ventu), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: EFEX (Ventu)
provider_slug: efex-ventu
slug: efex-ventu-domain-security
source_filename: efex-ventu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: efex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: efex.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/efex-ventu/refs/heads/main/security/efex-ventu-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Payments
- Cross-Border Payments
- Foreign Exchange
- Fintech
- Money Transfer
- Treasury
- Multi-Currency
- Mexico
---
