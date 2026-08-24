---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: kiddom.co
  spf: true
hosts:
- cert_expires: Oct 14 23:51:03 2026 GMT
  host: www.kiddom.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 02:30:09 2026 GMT
  host: get.kiddom.co
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 21 18:37:45 2026 GMT
  host: api.kiddom.co
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kiddom Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kiddom, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Kiddom
provider_slug: kiddom
slug: kiddom-domain-security
source_filename: kiddom-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kiddom.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 23:51:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: get.kiddom.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 02:30:09 2026 GMT\n  hsts: null\n- host: api.kiddom.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 18:37:45 2026 GMT\n  hsts: null\ndomains:\n- domain: kiddom.co\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kiddom/refs/heads/main/security/kiddom-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Education
- K-12
- Curriculum
- Learning Management
- Assessment
- EdTech
- Rostering
- Interoperability
- LTI
- OneRoster
- Analytics
---
