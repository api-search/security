---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: impossiblemetals.com
  spf: true
hosts:
- cert_expires: Sep 28 13:17:53 2026 GMT
  host: impossiblemetals.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Impossible Metals Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Impossible Metals, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Impossible Metals
provider_slug: impossible-metals
slug: impossible-metals-domain-security
source_filename: impossible-metals-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: impossiblemetals.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 13:17:53 2026 GMT\n  hsts: false\ndomains:\n- domain: impossiblemetals.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/impossible-metals/refs/heads/main/security/impossible-metals-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Deep Sea Mining
- Critical Minerals
- Battery Metals
- Robotics
- Autonomous Underwater Vehicles
- Ocean Technology
- Mining
- Sustainability
- Climate Tech
- Content
- Event
---
