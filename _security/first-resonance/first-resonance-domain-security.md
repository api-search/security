---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: firstresonance.io
  spf: true
- caa:
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: buildwithion.com
  spf: false
hosts:
- cert_expires: Sep 11 10:36:11 2026 GMT
  host: firstresonance.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  2 13:27:25 2026 GMT
  host: manual.firstresonance.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 22 16:15:20 2026 GMT
  host: api.buildwithion.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: First Resonance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for First Resonance, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: First Resonance
provider_slug: first-resonance
slug: first-resonance-domain-security
source_filename: first-resonance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: firstresonance.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 10:36:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: manual.firstresonance.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 13:27:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.buildwithion.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 16:15:20 2026 GMT\n  hsts: null\ndomains:\n- domain: firstresonance.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: buildwithion.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/first-resonance/refs/heads/main/security/first-resonance-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Infrastructure
- Manufacturing
- MES
- Factory Operating System
- Hardware
- Aerospace
- GraphQL
- Traceability
- Supply Chain
---
