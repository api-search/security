---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: changehealthcare.com
  spf: true
hosts:
- cert_expires: Dec  2 23:59:59 2026 GMT
  host: www.changehealthcare.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- host: developer.changehealthcare.com
  https: false
- host: api.changehealthcare.com
  https: false
kind: domain-security
layout: security
method: probed
name: Change Healthcare Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Change Healthcare, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Change Healthcare
provider_slug: change-healthcare
slug: change-healthcare-domain-security
source_filename: change-healthcare-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.changehealthcare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: developer.changehealthcare.com\n  https: false\n- host: api.changehealthcare.com\n  https: false\ndomains:\n- domain: changehealthcare.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/change-healthcare/refs/heads/main/security/change-healthcare-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Healthcare
- Technology
- Analytics
---
