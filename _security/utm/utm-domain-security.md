---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: utm.my
  spf: true
hosts:
- cert_expires: Aug 28 00:22:49 2026 GMT
  host: www.utm.my
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: eprints.utm.my
  https: false
kind: domain-security
layout: security
method: probed
name: Utm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Universiti Teknologi Malaysia, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Universiti Teknologi Malaysia
provider_slug: utm
slug: utm-domain-security
source_filename: utm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.utm.my\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 00:22:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: eprints.utm.my\n  https: false\ndomains:\n- domain: utm.my\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/utm/refs/heads/main/security/utm-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Research
- Open Access
- Institutional Repository
- OAI-PMH
- Malaysia
---
