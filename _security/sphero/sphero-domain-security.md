---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sphero.com
  spf: true
hosts:
- cert_expires: Aug 30 08:35:31 2026 GMT
  host: sphero.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sphero Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sphero, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sphero
provider_slug: sphero
slug: sphero-domain-security
source_filename: sphero-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sphero.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 08:35:31 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: sphero.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sphero/refs/heads/main/security/sphero-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Hardware
- Robotics
- Education
- STEAM
- SDK
- Robots
- EdTech
---
