---
description: ''
domains:
- caa:
  - 0 iodef "mailto:DL_IT_TS@stockland.com.au"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "amazon.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: stockland.com.au
  spf: true
hosts:
- cert_expires: Nov 10 23:59:59 2026 GMT
  host: stockland.com.au
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Stockland Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stockland, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Stockland
provider_slug: stockland
slug: stockland-domain-security
source_filename: stockland-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: stockland.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: stockland.com.au\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:DL_IT_TS@stockland.com.au\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stockland/refs/heads/main/security/stockland-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Real Estate
- Property Development
- Retail
- Logistics
- Residential
- Australia
---
