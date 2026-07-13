---
api_specs:
- filename: docs
  format: yaml
  label: yDaemon REST API
  slug: ydaemon-rest-api
  spec_type: OpenAPI
  url: https://ydaemon.yearn.fi/docs
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: yearn.fi
  spf: true
hosts:
- cert_expires: Sep 11 04:06:56 2026 GMT
  host: docs.yearn.fi
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 10:21:12 2026 GMT
  host: ydaemon.yearn.fi
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  7 04:34:17 2026 GMT
  host: kong.yearn.fi
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Yearn Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Yearn Finance, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Yearn Finance
provider_slug: yearn
slug: yearn-domain-security
source_filename: yearn-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.yearn.fi\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 04:06:56 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: ydaemon.yearn.fi\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 10:21:12 2026 GMT\n  hsts: null\n- host: kong.yearn.fi\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 04:34:17 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: yearn.fi\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yearn/refs/heads/main/security/yearn-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- DeFi
- Yield Aggregator
- Vaults
- EVM
- Web3
- Blockchain
- Finance
---
