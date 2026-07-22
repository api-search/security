---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: approva.co
  spf: true
hosts:
- cert_expires: Aug 19 18:13:01 2026 GMT
  host: approva.co
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Approva Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Approva, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Approva
provider_slug: approva
slug: approva-domain-security
source_filename: approva-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: approva.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 18:13:01 2026 GMT\n  hsts: false\ndomains:\n- domain: approva.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/approva/refs/heads/main/security/approva-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Fintech
- Mortgage
- Lending
- Marketplace
- Loans
- Brokers
---
