---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cabinethealth.com
  spf: true
hosts:
- cert_expires: Sep 29 20:24:48 2026 GMT
  host: cabinethealth.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cabinet Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cabinet Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cabinet Health
provider_slug: cabinet-health
slug: cabinet-health-domain-security
source_filename: cabinet-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cabinethealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 20:24:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cabinethealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cabinet-health/refs/heads/main/security/cabinet-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Pharmaceuticals
- Over-the-Counter Medicine
- Supply Chain
- Consumer Packaged Goods
- Sustainability
- Private Label
---
