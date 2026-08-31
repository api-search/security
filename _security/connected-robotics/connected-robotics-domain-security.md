---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: connected-robotics.com
  spf: true
hosts:
- cert_expires: Nov  7 23:59:59 2026 GMT
  host: connected-robotics.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Connected Robotics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Connected Robotics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Connected Robotics
provider_slug: connected-robotics
slug: connected-robotics-domain-security
source_filename: connected-robotics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: connected-robotics.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  7 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: connected-robotics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/connected-robotics/refs/heads/main/security/connected-robotics-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Robotics
- Foodtech
- Automation
- Artificial Intelligence
- Manufacturing
- Japan
---
