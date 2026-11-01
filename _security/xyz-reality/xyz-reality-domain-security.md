---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: xyzreality.com
  spf: true
hosts:
- cert_expires: Jan 20 22:43:41 2027 GMT
  host: www.xyzreality.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Xyz Reality Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for XYZ Reality, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: XYZ Reality
provider_slug: xyz-reality
slug: xyz-reality-domain-security
source_filename: xyz-reality-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.xyzreality.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 22:43:41 2027 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: xyzreality.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/xyz-reality/security/xyz-reality-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- RealEstate
- AR
- VR
- PropTech
- Platform
---
