---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: getsimma.com
  spf: true
hosts:
- cert_expires: Feb  8 23:59:59 2027 GMT
  host: getsimma.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Simma Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Simma, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Simma
provider_slug: getsimma-com
slug: getsimma-com-domain-security
source_filename: getsimma-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getsimma.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  8 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: getsimma.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/getsimma-com/security/getsimma-com-domain-security.yml
summary_line: TLSv1.3
tags:
- Endurance
- Coaching
- Artificial Intelligence
- Fitness
- Garmin
---
