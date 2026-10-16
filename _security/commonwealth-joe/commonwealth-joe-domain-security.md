---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: commonwealthjoe.com
  spf: true
hosts:
- cert_expires: Dec 27 20:03:33 2026 GMT
  host: commonwealthjoe.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Commonwealth Joe Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Commonwealth Joe, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Commonwealth Joe
provider_slug: commonwealth-joe
slug: commonwealth-joe-domain-security
source_filename: commonwealth-joe-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: commonwealthjoe.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 20:03:33 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: commonwealthjoe.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/commonwealth-joe/refs/heads/main/security/commonwealth-joe-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Coffee
- Retail
- Subscription
- Wholesale
- WashingtonDC
---
