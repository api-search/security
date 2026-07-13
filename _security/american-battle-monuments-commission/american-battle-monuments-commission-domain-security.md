---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: abmc.gov
  spf: true
hosts:
- cert_expires: Oct  3 23:59:59 2026 GMT
  host: www.abmc.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 11 23:59:59 2026 GMT
  host: weremember.abmc.gov
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: American Battle Monuments Commission Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for American Battle Monuments Commission, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: American Battle Monuments Commission
provider_slug: american-battle-monuments-commission
slug: american-battle-monuments-commission-domain-security
source_filename: american-battle-monuments-commission-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.abmc.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 23:59:59 2026 GMT\n  hsts: null\n- host: weremember.abmc.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: abmc.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/american-battle-monuments-commission/refs/heads/main/security/american-battle-monuments-commission-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Federal Government
- Military
- Veterans
- World War II
- Memorial
- Open Data
---
