---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: livongo.com
  spf: true
hosts:
- cert_expires: Aug  2 05:59:49 2026 GMT
  host: www.livongo.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Livongo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Livongo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Livongo
provider_slug: livongo
slug: livongo-domain-security
source_filename: livongo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.livongo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  2 05:59:49 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: livongo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/livongo/refs/heads/main/security/livongo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Digital Health
- Chronic Care
- Diabetes Management
- Remote Patient Monitoring
- Connected Devices
- Teladoc Health
---
