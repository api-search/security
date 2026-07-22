---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: perion.gg
  spf: true
hosts:
- cert_expires: Aug 29 22:02:59 2026 GMT
  host: perion.gg
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Perion Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Perion, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Perion
provider_slug: perion
slug: perion-domain-security
source_filename: perion-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: perion.gg\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 22:02:59 2026 GMT\n  hsts: null\ndomains:\n- domain: perion.gg\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/perion/refs/heads/main/security/perion-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Crypto
- Web3
- Blockchain
---
