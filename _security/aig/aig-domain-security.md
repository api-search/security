---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: aig.com
  spf: true
hosts:
- cert_expires: Feb 19 23:59:59 2027 GMT
  host: www.aig.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: myaig.aig.com
  https: false
- host: jobs.aig.com
  https: false
kind: domain-security
layout: security
method: probed
name: Aig Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AIG, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AIG
provider_slug: aig
slug: aig-domain-security
source_filename: aig-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aig.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 19 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: myaig.aig.com\n  https: false\n- host: jobs.aig.com\n  https: false\ndomains:\n- domain: aig.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aig/refs/heads/main/security/aig-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- Financial Services
- Property Casualty
- Cyber Insurance
- Enterprise
- Fortune 100
---
