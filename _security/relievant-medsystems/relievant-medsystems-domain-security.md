---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: relievant.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: intracept.com
  spf: true
hosts:
- cert_expires: Aug 21 16:21:49 2026 GMT
  host: www.relievant.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 29 23:59:59 2026 GMT
  host: www.intracept.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Relievant Medsystems Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Relievant Medsystems, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Relievant Medsystems
provider_slug: relievant-medsystems
slug: relievant-medsystems-domain-security
source_filename: relievant-medsystems-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.relievant.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 16:21:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.intracept.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: relievant.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: intracept.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/relievant-medsystems/refs/heads/main/security/relievant-medsystems-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Medical Devices
- Healthcare
- Medtech
- Pain Management
- Spine
- Neuromodulation
---
