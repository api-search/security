---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: tellroby.com
  spf: true
hosts:
- cert_expires: Mar  1 23:59:59 2027 GMT
  host: tellroby.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Roby Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Roby, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Roby
provider_slug: roby
slug: roby-domain-security
source_filename: roby-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tellroby.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  1 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: tellroby.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/roby/refs/heads/main/security/roby-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- HVAC
- Building Management
- Energy Efficiency
- Automation
- Facilities
- Sustainability
- Workplace
---
