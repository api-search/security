---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: indigoag.com
  spf: true
hosts:
- cert_expires: Sep 19 01:24:39 2026 GMT
  host: www.indigoag.com
  hsts: true
  hsts_max_age: 3628800
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 23:59:59 2026 GMT
  host: app.indigoag.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Indigo Ag Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Indigo Agriculture, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Indigo Agriculture
provider_slug: indigo-ag
slug: indigo-ag-domain-security
source_filename: indigo-ag-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.indigoag.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 01:24:39 2026 GMT\n  hsts: true\n  hsts_max_age: 3628800\n- host: app.indigoag.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: indigoag.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/indigo-ag/refs/heads/main/security/indigo-ag-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Agriculture
- AgTech
- Microbials
- Soil Carbon
- MRV
- Scope 3
- Sustainability
---
