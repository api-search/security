---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: tcgdex.net
  spf: true
hosts:
- cert_expires: Sep  1 21:30:50 2026 GMT
  host: www.tcgdex.net
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tcgdex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TCGdex, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: TCGdex
provider_slug: tcgdex
slug: tcgdex-domain-security
source_filename: tcgdex-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tcgdex.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 21:30:50 2026 GMT\n  hsts: null\ndomains:\n- domain: tcgdex.net\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tcgdex/refs/heads/main/security/tcgdex-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Games And Comics
- Public APIs
---
