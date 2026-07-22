---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: firstcash.com
  spf: true
hosts:
- cert_expires: Nov 21 18:03:33 2026 GMT
  host: www.firstcash.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Firstcash Holdings Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FirstCash Holdings, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: FirstCash Holdings
provider_slug: firstcash-holdings
slug: firstcash-holdings-domain-security
source_filename: firstcash-holdings-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.firstcash.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 18:03:33 2026 GMT\n  hsts: false\ndomains:\n- domain: firstcash.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/firstcash-holdings/refs/heads/main/security/firstcash-holdings-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Financial Services
- Pawn Loans
- Consumer Finance
- Retail
- Lease-to-Own
---
