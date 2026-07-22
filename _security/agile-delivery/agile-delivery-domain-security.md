---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: agilealliance.org
  spf: true
hosts:
- cert_expires: Aug 24 13:32:16 2026 GMT
  host: agilealliance.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Agile Delivery Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agile Delivery, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Agile Delivery
provider_slug: agile-delivery
slug: agile-delivery-domain-security
source_filename: agile-delivery-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agilealliance.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 13:32:16 2026 GMT\n  hsts: false\ndomains:\n- domain: agilealliance.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agile-delivery/refs/heads/main/security/agile-delivery-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Agile
- Iterative Development
- Project Management
- Software Development
- Sprint
- Scrum
---
