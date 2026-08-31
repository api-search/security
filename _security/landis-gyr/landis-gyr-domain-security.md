---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: landisgyr.com
  note: No DNSSEC and no CAA records. DMARC is enforced at p=quarantine rather than p=reject. Verified by dig on 2026-07-27.
  spf: true
hosts:
- cert_expires: Oct 12 00:26:14 2026 GMT
  host: www.landisgyr.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  2 18:54:11 2026 GMT
  host: toolsportal.landisgyr.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 25 10:24:45 2026 GMT
  host: developers.landisgyr.com
  hsts: true
  hsts_max_age: 31556926
  https: true
  note: Developer portal (Firebase Hosting).
  tls_version: TLSv1.3
- cert_expires: Sep 14 01:50:21 2026 GMT
  host: blog.landisgyr.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  note: HubSpot-hosted blog.
  tls_version: TLSv1.3
- cert_expires: Sep 13 05:38:36 2026 GMT
  host: investors.landisgyr.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Landis Gyr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Landis+Gyr, probed live across 5 host(s) and 1 registrable domain(s). 5 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Landis+Gyr
provider_slug: landis-gyr
slug: landis-gyr-domain-security
source_filename: landis-gyr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.landisgyr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 00:26:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: toolsportal.landisgyr.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep  2 18:54:11 2026 GMT\n  hsts: false\n- host: developers.landisgyr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 10:24:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\n  note: Developer portal (Firebase Hosting).\n- host: blog.landisgyr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 01:50:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  note: HubSpot-hosted blog.\n- host: investors.landisgyr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 05:38:36 2026 GMT\n  hsts: false\ndomains:\n- domain: landisgyr.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n\
  \  dmarc_policy: quarantine\n  note: >-\n    No DNSSEC and no CAA records. DMARC is enforced at p=quarantine rather than p=reject.\n    Verified by dig on 2026-07-27.\nnotes:\n- >-\n  toolsportal.landisgyr.com is the weakest host — TLS 1.2 with no HSTS — and it is the\n  customer login surface. Every other resolving host negotiates TLS 1.3.\n- >-\n  Hosts probed but excluded from the table: eu.landisgyr.com (EMEA property, divested to\n  AURELIUS in 2026) and careers.landisgyr.com (third-party jobs2web ATS).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/landis-gyr/refs/heads/main/security/landis-gyr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- United States
- Utilities
- Electricity
- Gas
- Water
- Smart Metering
- AMI
- Grid
- Grid Edge
- Demand Response
- Internet Of Things
- Meter Data Management
- Wi-SUN
- Energy Technology
---
