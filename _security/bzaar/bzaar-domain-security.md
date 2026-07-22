---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bzaar.com
  spf: true
hosts:
- cert_expires: Nov  9 15:38:02 2026 GMT
  host: bzaar.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bzaar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bzaar, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Bzaar
provider_slug: bzaar
slug: bzaar-domain-security
source_filename: bzaar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bzaar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 15:38:02 2026 GMT\n  hsts: false\ndomains:\n- domain: bzaar.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bzaar/refs/heads/main/security/bzaar-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- B2B
- Marketplace
- Wholesale
- E-Commerce
- Retail
- Cross-Border Trade
- Sourcing
- Supply Chain
- India
- Southeast Asia
---
