---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: solofunds.com
  spf: true
hosts:
- cert_expires: Sep 17 12:34:20 2026 GMT
  host: solofunds.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Solo Funds Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SoLo Funds, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: SoLo Funds
provider_slug: solo-funds
slug: solo-funds-domain-security
source_filename: solo-funds-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: solofunds.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 12:34:20 2026 GMT\n  hsts: false\ndomains:\n- domain: solofunds.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/solo-funds/refs/heads/main/security/solo-funds-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Financial Services
- Fintech
- Lending
- Peer-to-Peer
- Personal Finance
- Mobile
---
