---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: tranched.fi
  spf: true
hosts:
- cert_expires: Aug 24 08:07:25 2026 GMT
  host: tranched.fi
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tranched Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tranched, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Tranched
provider_slug: tranched
slug: tranched-domain-security
source_filename: tranched-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tranched.fi\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 08:07:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tranched.fi\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tranched/refs/heads/main/security/tranched-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Financial Services
- Fintech
- Securitization
- Asset-Based Finance
- Tokenization
- Blockchain
- Private Credit
- Capital Markets
- Lending
---
