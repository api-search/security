---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: renegadeinsurance.com
  spf: true
hosts:
- cert_expires: Oct 26 19:39:05 2026 GMT
  host: renegadeinsurance.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 18 23:59:59 2026 GMT
  host: api.renegadeinsurance.com
  hsts: false
  https: true
  note: live AWS ALB; answers 404 "Invalid Endpoint" on every probed path (no public contract, docs, or discovery document)
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Renegade Insurance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Renegade Insurance, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Renegade Insurance
provider_slug: renegade-insurance
slug: renegade-insurance-domain-security
source_filename: renegade-insurance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: renegadeinsurance.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 19:39:05 2026 GMT\n  hsts: false\n- host: api.renegadeinsurance.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 23:59:59 2026 GMT\n  hsts: false\n  note: live AWS ALB; answers 404 \"Invalid Endpoint\" on every probed path (no public\n    contract, docs, or discovery document)\ndomains:\n- domain: renegadeinsurance.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/renegade-insurance/refs/heads/main/security/renegade-insurance-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Insurance
- Property and Casualty
- Insurtech
- Insurance Agency
- Franchise
- Quoting
- Agent Platform
---
