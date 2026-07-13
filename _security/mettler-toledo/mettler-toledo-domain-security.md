---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mt.com
  spf: true
hosts:
- cert_expires: Dec  9 23:59:59 2026 GMT
  host: www.mt.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: developer.mt.com
  https: false
- host: api.mt.com
  https: false
kind: domain-security
layout: security
method: probed
name: Mettler Toledo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mettler-Toledo International, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Mettler-Toledo International
provider_slug: mettler-toledo
slug: mettler-toledo-domain-security
source_filename: mettler-toledo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 23:59:59 2026 GMT\n  hsts: null\n- host: developer.mt.com\n  https: false\n- host: api.mt.com\n  https: false\ndomains:\n- domain: mt.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mettler-toledo/refs/heads/main/security/mettler-toledo-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Laboratory
- Instruments
- Precision
- Fortune 1000
---
