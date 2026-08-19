---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: brigad.co
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: brigad.cloud
  spf: false
hosts:
- cert_expires: Oct  1 09:19:03 2026 GMT
  host: www.brigad.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 23:59:59 2026 GMT
  host: app.hsp.brigad.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  6 13:40:32 2026 GMT
  host: brigadhsp-router-talent-brigadhsp-prod.plat.euw1.prod.brigad.cloud
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Brigad Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Brigad, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Brigad
provider_slug: brigad
slug: brigad-domain-security
source_filename: brigad-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.brigad.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 09:19:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.hsp.brigad.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: brigadhsp-router-talent-brigadhsp-prod.plat.euw1.prod.brigad.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 13:40:32 2026 GMT\n  hsts: null\ndomains:\n- domain: brigad.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: brigad.cloud\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brigad/refs/heads/main/security/brigad-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Staffing
- Marketplace
- Hospitality
- Healthcare
- Gig Economy
- Freelance
- Workforce
---
