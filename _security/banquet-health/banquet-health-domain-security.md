---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: banquethealth.com
  spf: true
hosts:
- cert_expires: Dec 12 22:17:04 2026 GMT
  host: www.banquethealth.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Banquet Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Banquet Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Banquet Health
provider_slug: banquet-health
slug: banquet-health-domain-security
source_filename: banquet-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.banquethealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 22:17:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: banquethealth.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/banquet-health/refs/heads/main/security/banquet-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Food Service Management
- Hospital Software
- Meal Management
- Healthcare Analytics
- Clinical Nutrition
---
