---
description: ''
domains:
- caa:
  - ;; connection timed out; no servers could be reached
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: yardi.com
  spf: true
hosts:
- cert_expires: Oct  6 02:36:40 2026 GMT
  host: www.yardi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Yardi Propware Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Yardi Propware, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Yardi Propware
provider_slug: yardi-propware
slug: yardi-propware-domain-security
source_filename: yardi-propware-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.yardi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 02:36:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: yardi.com\n  dnssec: false\n  caa:\n  - ;; connection timed out; no servers could be reached\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yardi-propware/refs/heads/main/security/yardi-propware-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Accounting
- Commercial
- Leasing
- Property Management
- Real Estate
- Residential
- Yardi
---
