---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: carsome.my
  spf: true
hosts:
- cert_expires: Aug 25 21:15:08 2026 GMT
  host: carsome.my
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Carsome Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Carsome, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Carsome
provider_slug: carsome
slug: carsome-domain-security
source_filename: carsome-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: carsome.my\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 21:15:08 2026 GMT\n  hsts: null\ndomains:\n- domain: carsome.my\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carsome/refs/heads/main/security/carsome-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Automotive
- E-Commerce
- Marketplace
- Used Cars
- Automotive Finance
- Southeast Asia
- Malaysia
---
