---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: workplaced.com
  spf: true
hosts:
- cert_expires: Dec  9 23:59:59 2026 GMT
  host: workplaced.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Workplaced Technologies Ltd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Workplaced Technologies Ltd, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Workplaced Technologies Ltd
provider_slug: workplaced-technologies-ltd
slug: workplaced-technologies-ltd-domain-security
source_filename: workplaced-technologies-ltd-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: workplaced.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: workplaced.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workplaced-technologies-ltd/refs/heads/main/security/workplaced-technologies-ltd-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Workplace
- Hybrid Work
- Occupancy
- Desk Booking
- Workplace Analytics
- Real Estate
- SaaS
---
