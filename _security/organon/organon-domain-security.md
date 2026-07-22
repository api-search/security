---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: organon.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: organonpro.com
  spf: true
hosts:
- cert_expires: Sep 25 06:47:48 2026 GMT
  host: www.organon.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 16:09:44 2026 GMT
  host: www.organonpro.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Organon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Organon, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Organon
provider_slug: organon
slug: organon-domain-security
source_filename: organon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.organon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 06:47:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.organonpro.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 16:09:44 2026 GMT\n  hsts: false\ndomains:\n- domain: organon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: organonpro.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/organon/refs/heads/main/security/organon-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fortune 500
- Healthcare
- Pharmaceuticals
- Womens Health
- Biosimilars
---
