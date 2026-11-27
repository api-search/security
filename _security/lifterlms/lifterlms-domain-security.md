---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lifterlms.com
  spf: true
hosts:
- cert_expires: Feb  6 11:12:21 2027 GMT
  host: lifterlms.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Lifterlms Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lifterlms, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Lifterlms
provider_slug: lifterlms
slug: lifterlms-domain-security
source_filename: lifterlms-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lifterlms.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  6 11:12:21 2027 GMT\n  hsts: false\ndomains:\n- domain: lifterlms.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/lifterlms/security/lifterlms-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- WordPress Plugin
- Online Courses
- Membership Training
- Education Technology
- Course Creation
---
