---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: causera.com
  spf: false
hosts:
- cert_expires: Nov  9 08:08:32 2026 GMT
  host: causera.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Causera Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Causera, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Causera
provider_slug: causera
slug: causera-domain-security
source_filename: causera-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: causera.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 08:08:32 2026 GMT\n  hsts: false\ndomains:\n- domain: causera.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/causera/refs/heads/main/security/causera-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Startup
- 500 Global
- Portfolio
- Defunct
- Palo Alto
- No API Surface
---
