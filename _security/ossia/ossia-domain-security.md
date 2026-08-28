---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ossia.com
  spf: true
hosts:
- cert_expires: Nov 18 23:39:49 2026 GMT
  host: www.ossia.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ossia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ossia, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Ossia
provider_slug: ossia
slug: ossia-domain-security
source_filename: ossia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ossia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 18 23:39:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ossia.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ossia/refs/heads/main/security/ossia-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Wireless Power
- Wireless Charging
- RF Energy
- Power over Air
- Hardware
- Semiconductors
- Internet of Things
- IoT Sensors
- Consumer Electronics
- Automotive
- Technology Licensing
- Deep Tech
- Washington
---
