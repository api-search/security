---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: intuitive.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: intuitive-surgical.com
  spf: false
hosts:
- cert_expires: Aug  3 22:14:19 2026 GMT
  host: www.intuitive.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: www.intuitive-surgical.com
  https: false
kind: domain-security
layout: security
method: probed
name: Intuitive Surgical Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Intuitive Surgical, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Intuitive Surgical
provider_slug: intuitive-surgical
slug: intuitive-surgical-domain-security
source_filename: intuitive-surgical-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.intuitive.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  3 22:14:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.intuitive-surgical.com\n  https: false\ndomains:\n- domain: intuitive.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: intuitive-surgical.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/intuitive-surgical/refs/heads/main/security/intuitive-surgical-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Robotic Surgery
- Medical Devices
- Healthcare
- Surgery
- da Vinci
- Fortune 500
---
