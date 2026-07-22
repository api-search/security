---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: trybaker.com
  spf: true
hosts:
- cert_expires: Jan  3 15:50:01 2027 GMT
  host: trybaker.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Baker Technologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Baker Technologies, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Baker Technologies
provider_slug: baker-technologies
slug: baker-technologies-domain-security
source_filename: baker-technologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: trybaker.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 15:50:01 2027 GMT\n  hsts: false\ndomains:\n- domain: trybaker.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/baker-technologies/refs/heads/main/security/baker-technologies-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Cannabis
- CRM
- Marketing
- Dispensary
- Loyalty
- Online Ordering
- Analytics
- Defunct
---
