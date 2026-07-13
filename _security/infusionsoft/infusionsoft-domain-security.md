---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: keap.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: infusionsoft.com
  spf: true
hosts:
- cert_expires: Sep 15 13:11:32 2026 GMT
  host: keap.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  7 13:21:01 2026 GMT
  host: developer.infusionsoft.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 22:11:50 2026 GMT
  host: api.infusionsoft.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Infusionsoft Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Infusionsoft (Keap), probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Infusionsoft (Keap)
provider_slug: infusionsoft
slug: infusionsoft-domain-security
source_filename: infusionsoft-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: keap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 13:11:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.infusionsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 13:21:01 2026 GMT\n  hsts: false\n- host: api.infusionsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 22:11:50 2026 GMT\n  hsts: null\ndomains:\n- domain: keap.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: infusionsoft.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/infusionsoft/refs/heads/main/security/infusionsoft-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- CRM
- Marketing Automation
- Sales Automation
- Email Marketing
- E-Commerce
- Small Business
---
