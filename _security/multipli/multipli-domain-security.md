---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: multipli.fi
  spf: true
hosts:
- cert_expires: Sep 21 15:07:03 2026 GMT
  host: multipli.fi
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Multipli Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Multipli, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Multipli
provider_slug: multipli
slug: multipli-domain-security
source_filename: multipli-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: multipli.fi\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 15:07:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: multipli.fi\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/multipli/refs/heads/main/security/multipli-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Crypto
- DeFi
- Stablecoin
- Yield
- Real World Assets
- Tokenization
- Blockchain
- EVM
- Web3
---
