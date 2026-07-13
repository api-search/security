---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: isevenapi.xyz
  spf: false
hosts:
- cert_expires: Sep 14 21:47:47 2026 GMT
  host: isevenapi.xyz
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Iseven Humor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for isEven (humor), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: isEven (humor)
provider_slug: iseven-humor
slug: iseven-humor-domain-security
source_filename: iseven-humor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: isevenapi.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 21:47:47 2026 GMT\n  hsts: false\ndomains:\n- domain: isevenapi.xyz\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/iseven-humor/refs/heads/main/security/iseven-humor-domain-security.yml
summary_line: TLSv1.3
tags:
- Science And Math
- Public APIs
---
