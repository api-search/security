---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: wag-art.com
  spf: true
hosts:
- cert_expires: Dec  7 14:35:22 2026 GMT
  host: www.wag-art.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Artory Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Artory, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Artory
provider_slug: artory
slug: artory-domain-security
source_filename: artory-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wag-art.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 14:35:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: wag-art.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/artory/refs/heads/main/security/artory-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Art
- Marketplace
- Data
- AssetManagement
---
