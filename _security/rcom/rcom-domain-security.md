---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: rcom.co.in
  spf: true
hosts:
- cert_expires: Oct  6 09:45:01 2026 GMT
  host: rcom.co.in
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Rcom Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rcom, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Rcom
provider_slug: rcom
slug: rcom-domain-security
source_filename: rcom-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rcom.co.in\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  6 09:45:01 2026 GMT\n  hsts: false\ndomains:\n- domain: rcom.co.in\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rcom/refs/heads/main/security/rcom-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Telecommunications
- Enterprise
- Networking
- Data Center
- Cloud
- Connectivity
- Voice
- India
---
