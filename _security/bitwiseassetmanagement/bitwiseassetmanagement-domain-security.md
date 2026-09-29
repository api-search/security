---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: bitwiseinvestments.com
  spf: true
hosts:
- cert_expires: Dec 20 16:40:50 2026 GMT
  host: bitwiseinvestments.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bitwiseassetmanagement Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bitwiseassetmanagement, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Bitwiseassetmanagement
provider_slug: bitwiseassetmanagement
slug: bitwiseassetmanagement-domain-security
source_filename: bitwiseassetmanagement-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bitwiseinvestments.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 16:40:50 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: bitwiseinvestments.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bitwiseassetmanagement/refs/heads/main/security/bitwiseassetmanagement-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Crypto
- ETFs
- Investment
- Asset Management
---
