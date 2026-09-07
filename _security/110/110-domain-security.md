---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: 1-10.com
  spf: true
hosts:
- cert_expires: Oct 27 02:14:59 2026 GMT
  host: www.1-10.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: 110 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 1→10, Inc., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: 1→10, Inc.
provider_slug: '110'
slug: 110-domain-security
source_filename: 110-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.1-10.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 02:14:59 2026 GMT\n  hsts: false\ndomains:\n- domain: 1-10.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/110/refs/heads/main/security/110-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Creative Technology
- Experience Design
- XR
- Artificial Intelligence
- Projection Mapping
- Sensors
- Prototyping
- Japan
- Entertainment
- Company
---
