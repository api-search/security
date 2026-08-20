---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ceracare.co.uk
  spf: true
hosts:
- cert_expires: Aug 28 16:32:59 2026 GMT
  host: ceracare.co.uk
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cera Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cera, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cera
provider_slug: cera
slug: cera-domain-security
source_filename: cera-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ceracare.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 16:32:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: ceracare.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cera/refs/heads/main/security/cera-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Healthcare
- United Kingdom
- Telehealth
- Home Care
- Remote Monitoring
- Digital Health
- Elderly Care
- Machine-Learning
---
