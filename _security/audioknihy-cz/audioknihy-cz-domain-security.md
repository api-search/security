---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: audioknihy.cz
  spf: false
hosts:
- cert_expires: Dec  2 08:06:55 2026 GMT
  host: audioknihy.cz
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Audioknihy Cz Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Audioknihy.cz, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Audioknihy.cz
provider_slug: audioknihy-cz
slug: audioknihy-cz-domain-security
source_filename: audioknihy-cz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: audioknihy.cz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 08:06:55 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: audioknihy.cz\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/audioknihy-cz/security/audioknihy-cz-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Audio
- Books
- Comparison
- Czech
- Marketplace
---
