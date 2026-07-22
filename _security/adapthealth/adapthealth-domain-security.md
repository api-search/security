---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: adapthealth.com
  spf: true
hosts:
- cert_expires: Sep 23 17:10:03 2026 GMT
  host: www.adapthealth.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Adapthealth Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AdaptHealth, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AdaptHealth
provider_slug: adapthealth
slug: adapthealth-domain-security
source_filename: adapthealth-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.adapthealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 17:10:03 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: adapthealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adapthealth/refs/heads/main/security/adapthealth-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Healthcare
- Medical Equipment
- Home Healthcare
- Respiratory Care
- Diabetes Care
---
