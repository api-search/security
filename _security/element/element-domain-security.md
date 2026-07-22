---
description: ''
domains:
- caa: []
  dmarc: true
  dnssec: true
  domain: element.fi
  spf: false
hosts:
- cert_expires: Sep 15 04:17:25 2026 GMT
  host: element.fi
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Element Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Element, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present.'
provider_name: Element
provider_slug: element
slug: element-domain-security
source_filename: element-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: element.fi\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 04:17:25 2026 GMT\n  hsts: null\ndomains:\n- domain: element.fi\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: true\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/element/refs/heads/main/security/element-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- DeFi
- Decentralized Finance
- Fixed Income
- Yield
- Ethereum
- Smart Contracts
- Cryptocurrency
- Governance
- DAO
---
