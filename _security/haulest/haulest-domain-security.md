---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: haulest.com
  spf: true
hosts:
- cert_expires: Dec 27 07:02:47 2026 GMT
  host: haulest.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Haulest Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Haulest, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Haulest
provider_slug: haulest
slug: haulest-domain-security
source_filename: haulest-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: haulest.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 07:02:47 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: haulest.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/haulest/refs/heads/main/security/haulest-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Moving
- Relocation
- Cost Estimation
- MCP
- Movers
- Consumer
---
