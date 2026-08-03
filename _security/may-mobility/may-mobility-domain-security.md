---
description: ''
domains:
- caa:
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: maymobility.com
  spf: true
hosts:
- cert_expires: Oct  8 04:46:23 2026 GMT
  host: maymobility.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 00:26:35 2026 GMT
  host: docs.maymobility.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: May Mobility Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for May Mobility, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: May Mobility
provider_slug: may-mobility
slug: may-mobility-domain-security
source_filename: may-mobility-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: maymobility.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 04:46:23 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: docs.maymobility.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 00:26:35 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: maymobility.com\n  dnssec: true\n  caa:\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/may-mobility/refs/heads/main/security/may-mobility-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Autonomous Vehicles
- Transportation
- Mobility
- Robotaxi
- Fleet Management
- Telemetry
- Public Transit
- Automotive
- Streaming
---
