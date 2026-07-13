---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: labcorp.com
  spf: true
hosts:
- cert_expires: Sep 26 11:26:12 2026 GMT
  host: www.labcorp.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Laboratory Corp Of America Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Laboratory Corporation of America (Labcorp), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Laboratory Corporation of America (Labcorp)
provider_slug: laboratory-corp-of-america
slug: laboratory-corp-of-america-domain-security
source_filename: laboratory-corp-of-america-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.labcorp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 11:26:12 2026 GMT\n  hsts: null\ndomains:\n- domain: labcorp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/laboratory-corp-of-america/refs/heads/main/security/laboratory-corp-of-america-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Alias
- Diagnostics
- FHIR
- Fortune 500
- Healthcare
- Laboratory
- Life Sciences
---
