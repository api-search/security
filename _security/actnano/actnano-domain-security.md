---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: actnano.com
  spf: true
hosts:
- cert_expires: Oct 17 18:20:35 2026 GMT
  host: actnano.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Actnano Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for actnano, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: actnano
provider_slug: actnano
slug: actnano-domain-security
source_filename: actnano-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: actnano.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 18:20:35 2026 GMT\n  hsts: false\ndomains:\n- domain: actnano.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/actnano/refs/heads/main/security/actnano-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Advanced Materials
- Nanotechnology
- Coatings
- Electronics Manufacturing
- Automotive
- Consumer Electronics
- Data Center Infrastructure
- Solar
- Medical Devices
- Manufacturing
---
