---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: srsacquiom.com
  spf: true
hosts:
- cert_expires: Oct 15 16:13:31 2026 GMT
  host: srsacquiom.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Srsacquiom Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SRS Acquiom, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: SRS Acquiom
provider_slug: srsacquiom
slug: srsacquiom-domain-security
source_filename: srsacquiom-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: srsacquiom.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 16:13:31 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: srsacquiom.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/srsacquiom/refs/heads/main/security/srsacquiom-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Mergers and Acquisitions
- Financial Services
- Escrow
- Payments
- Loan Agency
- Fintech
---
