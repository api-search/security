---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: flowbird.group
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: flowbirdhub.com
  spf: false
hosts:
- cert_expires: Sep  4 17:20:37 2026 GMT
  host: www.flowbird.group
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 02:55:52 2026 GMT
  host: docs.flowbirdhub.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Flowbird Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flowbird, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Flowbird
provider_slug: flowbird
slug: flowbird-domain-security
source_filename: flowbird-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.flowbird.group\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 17:20:37 2026 GMT\n  hsts: false\n- host: docs.flowbirdhub.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 02:55:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: flowbird.group\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: flowbirdhub.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flowbird/refs/heads/main/security/flowbird-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Parking
- Urban Mobility
- Transit Ticketing
- Payments
- Smart City
- Pay Stations
- EV Charging
- Digital Permits
- Partner Gated
---
