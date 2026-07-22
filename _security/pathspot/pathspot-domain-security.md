---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: pathspot.com
  spf: true
hosts:
- cert_expires: Oct 17 08:00:36 2026 GMT
  host: pathspot.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pathspot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PathSpot, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: PathSpot
provider_slug: pathspot
slug: pathspot-domain-security
source_filename: pathspot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pathspot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 08:00:36 2026 GMT\n  hsts: false\ndomains:\n- domain: pathspot.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pathspot/refs/heads/main/security/pathspot-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Food Safety
- Hand Hygiene
- Restaurant Technology
- Food Service
- Compliance
- Temperature Monitoring
- IoT
---
