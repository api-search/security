---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: vay.io
  spf: true
hosts:
- cert_expires: Sep 29 21:42:01 2026 GMT
  host: vay.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vay, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Vay
provider_slug: vay
slug: vay-domain-security
source_filename: vay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vay.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 21:42:01 2026 GMT\n  hsts: false\ndomains:\n- domain: vay.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vay/refs/heads/main/security/vay-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Mobility
- Teledriving
- Remote Driving
- Car Rental
- Automotive
- Transportation
---
