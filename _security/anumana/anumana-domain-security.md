---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: anumana.ai
  spf: true
hosts:
- cert_expires: Oct 30 16:52:43 2026 GMT
  host: anumana.ai
  hsts: false
  https: true
  role: marketing website
  tls_version: TLSv1.3
- cert_expires: Nov 25 13:14:17 2026 GMT
  host: api.anumana.ai
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 63072000
  hsts_preload: true
  https: true
  role: authenticated platform application (nferx); every path redirects to /auth/signin/
  tls_version: TLSv1.3
- cert_expires: Oct  4 19:36:11 2026 GMT
  host: trust.anumana.ai
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  role: Vanta-hosted trust center
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Anumana Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Anumana, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Anumana
provider_slug: anumana
slug: anumana-domain-security
source_filename: anumana-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml hosts\nhosts:\n- host: anumana.ai\n  role: marketing website\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 16:52:43 2026 GMT\n  hsts: false\n- host: api.anumana.ai\n  role: authenticated platform application (nferx); every path redirects to /auth/signin/\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 13:14:17 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  hsts_include_subdomains: true\n  hsts_preload: true\n- host: trust.anumana.ai\n  role: Vanta-hosted trust center\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 19:36:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\ndomains:\n- domain: anumana.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\nnotes:\n- The apex marketing host anumana.ai does not send HSTS; the application host api.anumana.ai\n  sends a two-year HSTS\
  \ with includeSubDomains and preload.\n- No CAA records are published for anumana.ai. Absence is recorded data, not an error.\n- anumana.com does not resolve; anumana.ai is the operating domain.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anumana/refs/heads/main/security/anumana-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Artificial Intelligence
- Machine-Learning
- Medical Devices
- Cardiology
- Diagnostics
- Clinical Decision Support
- ECG
- Digital Health
---
