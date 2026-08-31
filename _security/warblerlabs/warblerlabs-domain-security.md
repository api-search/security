---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: warblerlabs.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: goldfinch.finance
  spf: true
hosts:
- host: warblerlabs.com
  https: false
- cert_expires: Sep 23 04:41:54 2026 GMT
  host: dev.goldfinch.finance
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 01:54:43 2026 GMT
  host: api.goldsky.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Warblerlabs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Warblerlabs, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Warblerlabs
provider_slug: warblerlabs
slug: warblerlabs-domain-security
source_filename: warblerlabs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: warblerlabs.com\n  https: false\n- host: dev.goldfinch.finance\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 04:41:54 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.goldsky.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 01:54:43 2026 GMT\n  hsts: null\ndomains:\n- domain: warblerlabs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: goldfinch.finance\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/warblerlabs/refs/heads/main/security/warblerlabs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Blockchain
- DeFi
- Fintech
- Credit
- Lending
- GraphQL
- Ethereum
- Web3
- Real-World Assets
- Identity
---
