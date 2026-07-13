---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tranetechnologies.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: trane.com
  spf: true
hosts:
- cert_expires: Nov  4 23:59:59 2026 GMT
  host: www.tranetechnologies.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 17:47:07 2026 GMT
  host: developer.devops.chvac.trane.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 23:59:59 2026 GMT
  host: www.trane.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Trane Technologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Trane Technologies, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Trane Technologies
provider_slug: trane-technologies
slug: trane-technologies-domain-security
source_filename: trane-technologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tranetechnologies.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: developer.devops.chvac.trane.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 17:47:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.trane.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\ndomains:\n- domain: tranetechnologies.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: trane.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trane-technologies/refs/heads/main/security/trane-technologies-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- HVAC
- Cold Chain
- Telematics
- Building Automation
- IoT
- Refrigeration
- Transport Refrigeration
- BACnet
- Smart Buildings
- Fortune 500
---
