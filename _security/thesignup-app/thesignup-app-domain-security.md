---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dns_aid:
    checked: '2026-11-26'
    published: false
  dnssec: false
  domain: thesignup.app
  spf: true
hosts:
- cert_expires: Jan 25 05:36:29 2027 GMT
  host: thesignup.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: TheSignup Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TheSignup, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: TheSignup
provider_slug: thesignup-app
slug: thesignup-app-domain-security
source_filename: thesignup-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: thesignup.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 25 05:36:29 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: thesignup.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n  dns_aid:\n    checked: '2026-11-26'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/thesignup-app/security/thesignup-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Event Signups
- Potluck
- Class Parties
- No‑App Signups
---
