---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gpsinsight.com
  spf: true
hosts:
- cert_expires: Nov 24 18:50:53 2026 GMT
  host: www.gpsinsight.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Gps Insight Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GPS Insight, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: GPS Insight
provider_slug: gps-insight
slug: gps-insight-domain-security
source_filename: gps-insight-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gpsinsight.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 18:50:53 2026 GMT\n  hsts: false\ndomains:\n- domain: gpsinsight.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gps-insight/refs/heads/main/security/gps-insight-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Fleet Management
- GPS Tracking
- Telematics
- Software-as-a-Service
---
