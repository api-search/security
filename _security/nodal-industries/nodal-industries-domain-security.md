---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nodalsecurity.com
  spf: true
hosts:
- cert_expires: Oct  3 01:57:56 2026 GMT
  host: nodalsecurity.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nodal Industries Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nodal Industries, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Nodal Industries
provider_slug: nodal-industries
slug: nodal-industries-domain-security
source_filename: nodal-industries-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nodalsecurity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 01:57:56 2026 GMT\n  hsts: false\ndomains:\n- domain: nodalsecurity.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nodal-industries/refs/heads/main/security/nodal-industries-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Security
- Network Security
- Cybersecurity
- Threat Intelligence
- Consumer Hardware
- IoT
- Appliance
---
