---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: potion.fi
  spf: false
hosts:
- cert_expires: Oct 14 06:59:53 2026 GMT
  host: potion.fi
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Potion Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Potion Labs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Potion Labs
provider_slug: potion-labs
slug: potion-labs-domain-security
source_filename: potion-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: potion.fi\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 06:59:53 2026 GMT\n  hsts: false\ndomains:\n- domain: potion.fi\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/potion-labs/refs/heads/main/security/potion-labs-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Defi
- Options
- Smart Contracts
- Ethereum
- Web3
- Risk Management
- Insurance
- Blockchain
---
