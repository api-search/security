---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: golden.ventures
  spf: true
hosts:
- cert_expires: Sep 30 08:00:17 2026 GMT
  host: www.golden.ventures
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Golden Ventures Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Golden Ventures, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Golden Ventures
provider_slug: golden-ventures
slug: golden-ventures-domain-security
source_filename: golden-ventures-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.golden.ventures\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 08:00:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: golden.ventures\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/golden-ventures/refs/heads/main/security/golden-ventures-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Venture Capital
- Seed Stage
- Startups
- Investment
- Pre-Seed
- Toronto
---
