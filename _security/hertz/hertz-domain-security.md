---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: hertz.com
  spf: true
hosts:
- cert_expires: Dec  9 12:31:16 2026 GMT
  host: www.hertz.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Hertz Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hertz, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Hertz
provider_slug: hertz
slug: hertz-domain-security
source_filename: hertz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hertz.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 12:31:16 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: hertz.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hertz/refs/heads/main/security/hertz-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Fortune 500
- Car Rental
- Vehicle Rental
- Travel
- Mobility
- Transportation
- Fleet Management
---
