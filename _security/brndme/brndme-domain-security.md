---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: brndme.in
  spf: false
hosts:
- cert_expires: Oct  7 06:34:35 2026 GMT
  host: brndme.in
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Brndme Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BRND.ME, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: BRND.ME
provider_slug: brndme
slug: brndme-domain-security
source_filename: brndme-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: brndme.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 06:34:35 2026 GMT\n  hsts: false\ndomains:\n- domain: brndme.in\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brndme/refs/heads/main/security/brndme-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Consumer
- House of Brands
- D2C
- E-commerce
- Health
- Wellness
- Lifestyle
- Fashion
- India
---
