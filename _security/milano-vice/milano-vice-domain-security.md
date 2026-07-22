---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: milano-vice.de
  spf: true
hosts:
- cert_expires: Sep 25 02:20:41 2026 GMT
  host: www.milano-vice.de
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Milano Vice Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Milano Vice, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Milano Vice
provider_slug: milano-vice
slug: milano-vice-domain-security
source_filename: milano-vice-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.milano-vice.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 02:20:41 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: milano-vice.de\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/milano-vice/refs/heads/main/security/milano-vice-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Food Delivery
- Virtual Restaurant
- Cloud Kitchen
- Pizza
- Consumer
- Germany
---
