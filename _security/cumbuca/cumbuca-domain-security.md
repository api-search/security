---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cumbuca.com
  spf: true
hosts:
- cert_expires: Oct  2 17:28:04 2026 GMT
  host: cumbuca.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cumbuca Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cumbuca, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Cumbuca
provider_slug: cumbuca
slug: cumbuca-domain-security
source_filename: cumbuca-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cumbuca.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 17:28:04 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: cumbuca.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cumbuca/refs/heads/main/security/cumbuca-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Open Finance
- Pix
- Payments
- Banking
- Brazil
- Open Banking
- Financial Data
- MCP
---
