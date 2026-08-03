---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: lendbuzz.com
  spf: true
hosts:
- cert_expires: Oct 15 12:08:42 2026 GMT
  host: www.lendbuzz.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 28 06:04:14 2026 GMT
  host: app.lendbuzz.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.lendbuzz.com
  https: false
  note: DNS resolves (44.237.92.21, 35.162.221.233) but TCP 443 and 80 both time out from the public internet — not a publicly reachable API host
kind: domain-security
layout: security
method: probed
name: Lendbuzz Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lendbuzz, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Lendbuzz
provider_slug: lendbuzz
slug: lendbuzz-domain-security
source_filename: lendbuzz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lendbuzz.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 12:08:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.lendbuzz.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 06:04:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.lendbuzz.com\n  https: false\n  note: DNS resolves (44.237.92.21, 35.162.221.233) but TCP 443 and 80 both time out\n    from the public internet — not a publicly reachable API host\ndomains:\n- domain: lendbuzz.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lendbuzz/refs/heads/main/security/lendbuzz-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Auto Lending
- Automotive
- Financial Services
- Fintech
- Lending
- Credit
- Machine Learning
- Consumer Finance
- Dealers
---
