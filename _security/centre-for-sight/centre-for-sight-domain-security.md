---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: centreforsight.com
  spf: true
hosts:
- cert_expires: Dec 21 06:06:12 2026 GMT
  host: www.centreforsight.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Centre For Sight Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Centre for Sight, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Centre for Sight
provider_slug: centre-for-sight
slug: centre-for-sight-domain-security
source_filename: centre-for-sight-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.centreforsight.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 06:06:12 2026 GMT\n  hsts: false\ndomains:\n- domain: centreforsight.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/centre-for-sight/refs/heads/main/security/centre-for-sight-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Healthcare
- Ophthalmology
- EyeCare
- Medical
- United Kingdom
---
