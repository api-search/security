---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: carthera.eu
  spf: true
hosts:
- cert_expires: Nov 20 06:26:50 2026 GMT
  host: carthera.eu
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Carthera Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Carthera, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Carthera
provider_slug: carthera
slug: carthera-domain-security
source_filename: carthera-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: carthera.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 06:26:50 2026 GMT\n  hsts: false\ndomains:\n- domain: carthera.eu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carthera/refs/heads/main/security/carthera-domain-security.yml
summary_line: TLSv1.3
tags:
- MedTech
- Ultrasound
- Brain Disorders
- Clinical Stage
- France
- USA
---
