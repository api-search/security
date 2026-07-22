---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: kiddo.health
  spf: true
hosts:
- cert_expires: Sep  1 03:23:52 2026 GMT
  host: kiddo.health
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kiddowear Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for KiddoWear, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: KiddoWear
provider_slug: kiddowear
slug: kiddowear-domain-security
source_filename: kiddowear-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kiddo.health\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 03:23:52 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: kiddo.health\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kiddowear/refs/heads/main/security/kiddowear-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Health
- Healthcare
- Pediatrics
- Behavioral Health
- Digital Health
- Connected Care
- Remote Patient Monitoring
---
