---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: acevisiongroup.com
  spf: true
hosts:
- cert_expires: Oct 31 20:24:51 2026 GMT
  host: acevisiongroup.com
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Acevisiongroup Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ace Vision Group, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Ace Vision Group
provider_slug: acevisiongroup
slug: acevisiongroup-domain-security
source_filename: acevisiongroup-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: acevisiongroup.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 31 20:24:51 2026 GMT\n  hsts: false\ndomains:\n- domain: acevisiongroup.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acevisiongroup/refs/heads/main/security/acevisiongroup-domain-security.yml
summary_line: TLSv1.2 · DNSSEC · DMARC
tags:
- Company
- Medical Devices
- Ophthalmology
- Healthcare
- Lasers
- Medical Technology
- Life Sciences
- Presbyopia
---
