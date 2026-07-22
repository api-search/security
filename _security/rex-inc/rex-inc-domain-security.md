---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: rex.fit
  spf: true
hosts:
- cert_expires: Oct  1 00:10:48 2026 GMT
  host: www.rex.fit
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 23 06:12:46 2026 GMT
  host: rex.fit
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rex Inc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rex Inc, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Rex Inc
provider_slug: rex-inc
slug: rex-inc-domain-security
source_filename: rex-inc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rex.fit\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 00:10:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: rex.fit\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 06:12:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: rex.fit\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rex-inc/refs/heads/main/security/rex-inc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Health
- Fitness
- Nutrition
- Artificial Intelligence
- Computer Vision
- Wearables
- Y Combinator
---
