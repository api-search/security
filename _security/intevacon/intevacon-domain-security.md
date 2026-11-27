---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: intevacon.com
  spf: true
hosts:
- cert_expires: Dec  4 12:50:03 2026 GMT
  host: intevacon.com
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Intevacon Fleet Card Solutions LLC Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Intevacon Fleet Card Solutions LLC, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Intevacon Fleet Card Solutions LLC
provider_slug: intevacon
slug: intevacon-domain-security
source_filename: intevacon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: intevacon.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  4 12:50:03 2026 GMT\n  hsts: false\ndomains:\n- domain: intevacon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/intevacon/security/intevacon-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Fleet Card
- Petroleum
- Payments
- Fuel Network
---
