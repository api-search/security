---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lloyds.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: londonmarketgroup.co.uk
  spf: true
hosts:
- cert_expires: Dec  2 23:59:59 2026 GMT
  host: www.lloyds.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- host: developer.lloyds.com
  https: false
- cert_expires: Dec  2 23:59:59 2026 GMT
  host: api.londonmarketgroup.co.uk
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Lloyds Of London Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lloyd''s of London, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Lloyd's of London
provider_slug: lloyds-of-london
slug: lloyds-of-london-domain-security
source_filename: lloyds-of-london-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lloyds.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  2 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.lloyds.com\n  https: false\n- host: api.londonmarketgroup.co.uk\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  2 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: lloyds.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: londonmarketgroup.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lloyds-of-london/refs/heads/main/security/lloyds-of-london-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Insurance
- United Kingdom
- Reinsurance
- Specialty Insurance
- London Market
- Underwriting
- Claims
- Delegated Authority
- Broker
- Market Infrastructure
- Standards
- ACORD
---
