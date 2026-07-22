---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: erieinsurance.com
  spf: true
hosts:
- cert_expires: Oct 11 23:59:59 2026 GMT
  host: www.erieinsurance.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Erie Insurance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Erie Insurance, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Erie Insurance
provider_slug: erie-insurance
slug: erie-insurance-domain-security
source_filename: erie-insurance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.erieinsurance.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: erieinsurance.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/erie-insurance/refs/heads/main/security/erie-insurance-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Auto Insurance
- Fortune 500
- Home Insurance
- Insurance
---
