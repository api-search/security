---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ethena.fi
  spf: true
hosts:
- cert_expires: Sep 18 13:52:57 2026 GMT
  host: ethena.fi
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 14 07:04:00 2026 GMT
  host: docs.ethena.fi
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  4 05:05:20 2026 GMT
  host: public.api.ethena.fi
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ethena Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ethena Labs, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Ethena Labs
provider_slug: ethena-labs
slug: ethena-labs-domain-security
source_filename: ethena-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ethena.fi\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 13:52:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.ethena.fi\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 07:04:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: public.api.ethena.fi\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 05:05:20 2026 GMT\n  hsts: null\ndomains:\n- domain: ethena.fi\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ethena-labs/refs/heads/main/security/ethena-labs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Crypto
- Stablecoin
- DeFi
- Synthetic Dollar
- Minting
- Blockchain
- Ethereum
---
