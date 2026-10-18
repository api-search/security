---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: apyguard.com
  spf: true
hosts:
- cert_expires: Dec 10 19:56:50 2026 GMT
  host: apyguard.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Apyguard Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apyguard, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Apyguard
provider_slug: apyguard
slug: apyguard-domain-security
source_filename: apyguard-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: apyguard.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 19:56:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: apyguard.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apyguard/refs/heads/main/security/apyguard-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- API Security
- Developer Tools
- Software-as-a-Service
- Cloud
---
