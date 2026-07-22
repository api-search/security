---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: kyndryl.com
  spf: true
hosts:
- cert_expires: Sep 20 18:15:56 2026 GMT
  host: www.kyndryl.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kyndryl Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kyndryl, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Kyndryl
provider_slug: kyndryl
slug: kyndryl-domain-security
source_filename: kyndryl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kyndryl.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 18:15:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: kyndryl.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kyndryl/refs/heads/main/security/kyndryl-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fortune 500
- IT Services
- Managed Services
- Cloud
- Mainframe
- Cybersecurity
---
