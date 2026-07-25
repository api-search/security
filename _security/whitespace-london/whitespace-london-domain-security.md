---
api_specs:
- filename: whitespace-london-platform-openapi.yml
  format: yaml
  label: Whitespace Platform API
  slug: whitespace-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whitespace-london/refs/heads/main/openapi/whitespace-london-platform-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: whitespace.co.uk
  spf: true
hosts:
- cert_expires: Oct 10 03:14:52 2026 GMT
  host: www.whitespace.co.uk
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 12 23:59:59 2026 GMT
  host: apidocs.whitespace.co.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 12 23:59:59 2026 GMT
  host: sandbox.whitespace.co.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Whitespace London Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Whitespace, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Whitespace
provider_slug: whitespace-london
slug: whitespace-london-domain-security
source_filename: whitespace-london-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.whitespace.co.uk\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 10 03:14:52 2026 GMT\n  hsts: null\n- host: apidocs.whitespace.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: sandbox.whitespace.co.uk\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 12 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: whitespace.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/whitespace-london/refs/heads/main/security/whitespace-london-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Insurance
- United Kingdom
- Reinsurance
- Property and Casualty
- Insurtech
- Broker
- Underwriting
- Placing Platform
- London Market
- Lloyd's of London
- ACORD
- Market Infrastructure
---
