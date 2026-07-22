---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: wearecirca.com
  spf: true
hosts:
- cert_expires: Oct  9 00:50:38 2026 GMT
  host: wearecirca.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Circa Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Circa Labs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Circa Labs
provider_slug: circa-labs
slug: circa-labs-domain-security
source_filename: circa-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wearecirca.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 00:50:38 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: wearecirca.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/circa-labs/refs/heads/main/security/circa-labs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Proptech
- Rentals
- Wealth
- Financial Services
---
