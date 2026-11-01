---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bounceinfinity.com
  spf: true
hosts:
- cert_expires: Dec 22 08:17:56 2026 GMT
  host: bounceinfinity.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bounceinfinity Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bounce, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Bounce
provider_slug: bounceinfinity-com
slug: bounceinfinity-com-domain-security
source_filename: bounceinfinity-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bounceinfinity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 08:17:56 2026 GMT\n  hsts: false\ndomains:\n- domain: bounceinfinity.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/bounceinfinity-com/security/bounceinfinity-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Mobility
- Electric Vehicles
- India
- Scooters
---
