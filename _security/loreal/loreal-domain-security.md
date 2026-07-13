---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: loreal.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: modiface.com
  spf: true
hosts:
- cert_expires: Oct  7 04:14:19 2026 GMT
  host: www.loreal.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 23:00:54 2026 GMT
  host: modiface.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Loreal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for L''Oréal, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: L'Oréal
provider_slug: loreal
slug: loreal-domain-security
source_filename: loreal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.loreal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 04:14:19 2026 GMT\n  hsts: null\n- host: modiface.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 23:00:54 2026 GMT\n  hsts: false\ndomains:\n- domain: loreal.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: modiface.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/loreal/refs/heads/main/security/loreal-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Augmented Reality
- Beauty
- Beauty Tech
- Consumer Products
- Cosmetics
- Personal Care
---
