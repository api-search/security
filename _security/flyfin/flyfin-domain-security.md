---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: flyfin.tax
  spf: true
hosts:
- cert_expires: Dec  3 23:59:59 2026 GMT
  host: flyfin.tax
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Flyfin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FlyFin, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: FlyFin
provider_slug: flyfin
slug: flyfin-domain-security
source_filename: flyfin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: flyfin.tax\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: flyfin.tax\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flyfin/refs/heads/main/security/flyfin-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Consumer
- Tax
- Fintech
- Artificial Intelligence
- Accounting
- Freelance
- Self-Employed
---
