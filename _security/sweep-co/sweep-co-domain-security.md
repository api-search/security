---
description: ''
domains:
- caa:
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sweep.net
  spf: true
hosts:
- cert_expires: Sep 14 14:59:46 2026 GMT
  host: www.sweep.net
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sweep Co Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sweep, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Sweep
provider_slug: sweep-co
slug: sweep-co-domain-security
source_filename: sweep-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sweep.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 14:59:46 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: sweep.net\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sweep-co/refs/heads/main/security/sweep-co-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Sustainability
- Carbon Management
- Carbon Accounting
- ESG
- ESG Reporting
- Climate
- Greenhouse Gas
- GHG Protocol
- Scope 3 Emissions
- Financed Emissions
- CSRD
- ISSB
- SB 253
- TCFD
- SFDR
- CDP
- Supply Chain
- Value Chain
- Compliance
- Disclosure
- Audit
---
