---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: polychain.capital
  spf: true
hosts:
- cert_expires: Sep 15 07:37:18 2026 GMT
  host: polychain.capital
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Polychain Capital Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Polychain Capital, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Polychain Capital
provider_slug: polychain-capital
slug: polychain-capital-domain-security
source_filename: polychain-capital-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: polychain.capital\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 07:37:18 2026 GMT\n  hsts: false\ndomains:\n- domain: polychain.capital\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/polychain-capital/refs/heads/main/security/polychain-capital-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Venture Capital
- Cryptocurrency
- Blockchain
- Digital Assets
- Investment
- Web3
---
