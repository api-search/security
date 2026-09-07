---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: zspace.com
  spf: true
hosts:
- cert_expires: Oct 11 09:29:55 2026 GMT
  host: zspace.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 11 09:29:55 2026 GMT
  host: developer.zspace.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 11 09:29:55 2026 GMT
  host: api.zspace.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Zspace Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for zSpace, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: zSpace
provider_slug: zspace
slug: zspace-domain-security
source_filename: zspace-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zspace.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 09:29:55 2026 GMT\n  hsts: false\n- host: developer.zspace.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 09:29:55 2026 GMT\n  hsts: false\n- host: api.zspace.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 09:29:55 2026 GMT\n  hsts: null\ndomains:\n- domain: zspace.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zspace/refs/heads/main/security/zspace-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Education
- Augmented Reality
- Virtual Reality
- EdTech
- Hardware
- 3D
- Simulation
- Career and Technical Education
- Developer SDK
---
