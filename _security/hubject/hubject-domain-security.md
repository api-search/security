---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hubject.com
  spf: true
hosts:
- cert_expires: Jan  6 23:14:25 2027 GMT
  host: www.hubject.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Hubject Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hubject, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Hubject
provider_slug: hubject
slug: hubject-domain-security
source_filename: hubject-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hubject.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 23:14:25 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hubject.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hubject/refs/heads/main/security/hubject-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- E-Mobility
- EVCharging
- Interoperability
---
