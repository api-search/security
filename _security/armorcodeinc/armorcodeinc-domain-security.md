---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: armorcode.com
  spf: true
hosts:
- cert_expires: Nov 28 05:09:45 2026 GMT
  host: www.armorcode.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Armorcodeinc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Armorcodeinc, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Armorcodeinc
provider_slug: armorcodeinc
slug: armorcodeinc-domain-security
source_filename: armorcodeinc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.armorcode.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 05:09:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: armorcode.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/armorcodeinc/refs/heads/main/security/armorcodeinc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Security
- Artificial Intelligence
- Risk Management
- Exposure Management
---
