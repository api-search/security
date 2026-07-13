---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bnsf.com
  spf: true
hosts:
- cert_expires: Sep 14 19:46:14 2026 GMT
  host: www.bnsf.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov 11 14:36:02 2026 GMT
  host: api.bnsf.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 11 14:52:03 2026 GMT
  host: api-trial.bnsf.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bnsf Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BNSF, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: BNSF
provider_slug: bnsf
slug: bnsf-domain-security
source_filename: bnsf-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bnsf.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 14 19:46:14 2026 GMT\n  hsts: false\n- host: api.bnsf.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 14:36:02 2026 GMT\n  hsts: null\n- host: api-trial.bnsf.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 14:52:03 2026 GMT\n  hsts: null\ndomains:\n- domain: bnsf.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bnsf/refs/heads/main/security/bnsf-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Freight
- Railroad
- Shipping
- Trains
- Intermodal
- Logistics
---
