---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: embodyme.com
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: digiself.tech
  spf: true
hosts:
- cert_expires: Nov 25 23:59:59 2026 GMT
  host: company.embodyme.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 23:59:59 2026 GMT
  host: digiself.tech
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 30 23:59:59 2027 GMT
  host: api.digiself.tech
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Embodyme Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EmbodyMe, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: EmbodyMe
provider_slug: embodyme
slug: embodyme-domain-security
source_filename: embodyme-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: company.embodyme.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 23:59:59 2026 GMT\n  hsts: false\n- host: digiself.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 23:59:59 2026 GMT\n  hsts: false\n- host: api.digiself.tech\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 30 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: embodyme.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: digiself.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/embodyme/refs/heads/main/security/embodyme-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- Avatars
- Digital Humans
- Neural Rendering
- Face Tracking
- Generative AI
- Video Generation
- Real-Time
- Streaming
- SDK
---
