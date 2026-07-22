---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nickelytics.com
  spf: true
hosts:
- cert_expires: Oct  1 05:00:18 2026 GMT
  host: nickelytics.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nickelytics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nickelytics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Nickelytics
provider_slug: nickelytics
slug: nickelytics-domain-security
source_filename: nickelytics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nickelytics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 05:00:18 2026 GMT\n  hsts: null\ndomains:\n- domain: nickelytics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nickelytics/refs/heads/main/security/nickelytics-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Advertising
- OOH
- DOOH
- Programmatic Advertising
- Mobility
- Robotics
- Rideshare
- AdTech
---
