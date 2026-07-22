---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: traxretail.com
  spf: true
hosts:
- cert_expires: Oct  2 05:09:23 2026 GMT
  host: traxretail.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 13 01:22:29 2026 GMT
  host: www.apidoc.traxretail.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 29 13:30:35 2026 GMT
  host: services.traxretail.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Trax Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Trax, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Trax
provider_slug: trax
slug: trax-domain-security
source_filename: trax-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: traxretail.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 05:09:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.apidoc.traxretail.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 01:22:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\n- host: services.traxretail.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 13:30:35 2026 GMT\n  hsts: false\ndomains:\n- domain: traxretail.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trax/refs/heads/main/security/trax-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Enterprise
- Retail
- Computer Vision
- Image Recognition
- CPG
- Retail Execution
- Merchandising
- SaaS
---
