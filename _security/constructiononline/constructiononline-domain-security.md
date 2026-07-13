---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: constructiononline.com
  spf: true
hosts:
- cert_expires: Aug 29 23:59:59 2026 GMT
  host: www.constructiononline.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 19 09:17:39 2026 GMT
  host: us.constructiononline.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Constructiononline Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ConstructionOnline, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: ConstructionOnline
provider_slug: constructiononline
slug: constructiononline-domain-security
source_filename: constructiononline-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.constructiononline.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 29 23:59:59 2026 GMT\n  hsts: false\n- host: us.constructiononline.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 09:17:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: constructiononline.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/constructiononline/refs/heads/main/security/constructiononline-domain-security.yml
summary_line: TLSv1.2 · HSTS
tags:
- Construction
- Estimating
- Project Management
- Projects
- Scheduling
- Subcontractors
- Time Tracking
---
