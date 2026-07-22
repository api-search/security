---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: novasparks.com
  spf: true
hosts:
- cert_expires: Sep  1 10:21:24 2026 GMT
  host: novasparks.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Novasparks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NovaSparks, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: NovaSparks
provider_slug: novasparks
slug: novasparks-domain-security
source_filename: novasparks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: novasparks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 10:21:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: novasparks.com\n  dnssec: true\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/novasparks/refs/heads/main/security/novasparks-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Infrastructure Saas
- Financial Services
- Market Data
- FPGA
- Low Latency
- Trading
- Hardware
---
