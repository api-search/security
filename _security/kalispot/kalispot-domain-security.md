---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: kalispot.com
  spf: true
hosts:
- cert_expires: Aug 17 21:06:47 2026 GMT
  host: kalispot.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kalispot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for KaliSpot, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: KaliSpot
provider_slug: kalispot
slug: kalispot-domain-security
source_filename: kalispot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kalispot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 21:06:47 2026 GMT\n  hsts: null\ndomains:\n- domain: kalispot.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kalispot/refs/heads/main/security/kalispot-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Fintech
- Financial Services
- Payments
- Financial Inclusion
- Mobile Money
- ATM Network
- Banking
- Africa
---
