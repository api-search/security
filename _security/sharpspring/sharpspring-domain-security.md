---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sharpspring.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: constantcontact.com
  spf: true
hosts:
- cert_expires: Oct 29 11:02:31 2026 GMT
  host: sharpspring.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 28 13:01:01 2026 GMT
  host: knowledgebase.constantcontact.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  2 19:40:37 2027 GMT
  host: api.sharpspring.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sharpspring Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SharpSpring, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SharpSpring
provider_slug: sharpspring
slug: sharpspring-domain-security
source_filename: sharpspring-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sharpspring.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 11:02:31 2026 GMT\n  hsts: false\n- host: knowledgebase.constantcontact.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 13:01:01 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.sharpspring.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  2 19:40:37 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: sharpspring.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: constantcontact.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sharpspring/refs/heads/main/security/sharpspring-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Marketing
- Marketing Automation
- CRM
- Email Marketing
- Sales
- Leads
- Campaigns
- Automation
- Software-as-a-Service
---
