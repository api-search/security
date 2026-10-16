---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: celeatx.com
  spf: true
hosts:
- cert_expires: Nov 30 18:39:58 2026 GMT
  host: www.celeatx.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Celea Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Celea Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Celea Therapeutics
provider_slug: celea-therapeutics
slug: celea-therapeutics-domain-security
source_filename: celea-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.celeatx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 18:39:58 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: celeatx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/celea-therapeutics/refs/heads/main/security/celea-therapeutics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Biopharma
- Respiratory
- IPF
- Therapeutics
---
