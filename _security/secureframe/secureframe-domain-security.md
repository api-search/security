---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: secureframe.com
  spf: true
hosts:
- cert_expires: Aug  8 15:58:26 2026 GMT
  host: secureframe.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 07:29:23 2026 GMT
  host: developer.secureframe.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 07:29:23 2026 GMT
  host: api.secureframe.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Secureframe Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Secureframe, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Secureframe
provider_slug: secureframe
slug: secureframe-domain-security
source_filename: secureframe-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: secureframe.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  8 15:58:26 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.secureframe.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 07:29:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\n- host: api.secureframe.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 07:29:23 2026 GMT\n  hsts: null\ndomains:\n- domain: secureframe.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/secureframe/refs/heads/main/security/secureframe-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- GRC
- Compliance
- SOC 2
- ISO 27001
- Risk
---
