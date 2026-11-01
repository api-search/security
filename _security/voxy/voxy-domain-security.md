---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: voxy.com
  spf: true
hosts:
- cert_expires: Dec 13 07:18:19 2026 GMT
  host: voxy.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Voxy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Voxy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Voxy
provider_slug: voxy
slug: voxy-domain-security
source_filename: voxy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: voxy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 07:18:19 2026 GMT\n  hsts: false\ndomains:\n- domain: voxy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/voxy/security/voxy-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- LanguageLearning
- AI
- CorporateTraining
- Education
---
