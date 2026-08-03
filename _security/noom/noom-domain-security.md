---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: noom.com
  spf: true
hosts:
- cert_expires: Oct 11 20:49:16 2026 GMT
  host: www.noom.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 11 20:49:16 2026 GMT
  host: api.noom.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_preload: true
  https: true
  note: application host; every anonymous request returns HTTP 401 UNAUTHENTICATED
- cert_expires: Sep  9 19:47:34 2026 GMT
  host: trust.noom.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  note: Vanta-hosted trust center
- cert_expires: Oct 29 23:59:59 2026 GMT
  host: account.noom.com
  hsts: false
  https: true
- cert_expires: Jan 15 23:59:59 2027 GMT
  host: healthcare.noom.com
  hsts: false
  https: true
  note: single-page healthcare client application
kind: domain-security
layout: security
method: probed
name: Noom Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Noom, probed live across 5 host(s) and 1 registrable domain(s). 5 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Noom
provider_slug: noom
slug: noom-domain-security
source_filename: noom-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.noom.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 20:49:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.noom.com\n  https: true\n  cert_expires: Oct 11 20:49:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  hsts_preload: true\n  note: application host; every anonymous request returns HTTP 401 UNAUTHENTICATED\n- host: trust.noom.com\n  https: true\n  cert_expires: Sep  9 19:47:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  note: Vanta-hosted trust center\n- host: account.noom.com\n  https: true\n  cert_expires: Oct 29 23:59:59 2026 GMT\n  hsts: false\n- host: healthcare.noom.com\n  https: true\n  cert_expires: Jan 15 23:59:59 2027 GMT\n  hsts: false\n  note: single-page healthcare client application\ndomains:\n- domain: noom.com\n  dnssec:\
  \ false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/noom/refs/heads/main/security/noom-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Health
- Digital Health
- Weight Management
- Wellness
- Behavioral Health
- Telehealth
- Nutrition
- Consumer Health
- Mobile Applications
---
