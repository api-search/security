---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: genesisdigitalassets.com
  spf: false
hosts:
- cert_expires: Aug 26 23:02:53 2026 GMT
  host: genesisdigitalassets.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Genesis Digital Assets Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Genesis Digital Assets, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Genesis Digital Assets
provider_slug: genesis-digital-assets
slug: genesis-digital-assets-domain-security
source_filename: genesis-digital-assets-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: genesisdigitalassets.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 23:02:53 2026 GMT\n  hsts: false\ndomains:\n- domain: genesisdigitalassets.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/genesis-digital-assets/refs/heads/main/security/genesis-digital-assets-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Company
- Infrastructure
- Bitcoin
- Cryptocurrency
- Data Centers
- Mining
- High-Performance Computing
- Blockchain
---
