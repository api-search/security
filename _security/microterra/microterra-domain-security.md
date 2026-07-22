---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: microterra.com.mx
  spf: false
hosts:
- cert_expires: Sep 26 23:24:57 2026 GMT
  host: microterra.com.mx
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Microterra Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for microTERRA, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: microTERRA
provider_slug: microterra
slug: microterra-domain-security
source_filename: microterra-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: microterra.com.mx\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 23:24:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: microterra.com.mx\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microterra/refs/heads/main/security/microterra-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Food
- Food and Beverage
- Ingredients
- Sustainability
- Biotechnology
- Agriculture
---
