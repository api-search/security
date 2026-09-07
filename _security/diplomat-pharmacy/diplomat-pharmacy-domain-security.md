---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: diplomatpharmacy.com
  spf: true
hosts:
- cert_expires: Dec 30 23:59:59 2026 GMT
  host: diplomatpharmacy.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Diplomat Pharmacy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Diplomat Pharmacy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Diplomat Pharmacy
provider_slug: diplomat-pharmacy
slug: diplomat-pharmacy-domain-security
source_filename: diplomat-pharmacy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: diplomatpharmacy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: diplomatpharmacy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/diplomat-pharmacy/refs/heads/main/security/diplomat-pharmacy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Healthcare
- Pharmacy
- Specialty Pharmacy
- Pharmaceuticals
- Fortune 1000
---
