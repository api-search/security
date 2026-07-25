---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: theclearinghouse.org
  spf: true
hosts:
- cert_expires: Oct 27 23:59:59 2026 GMT
  host: www.theclearinghouse.org
  hsts: true
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: The Clearing House Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The Clearing House (RTP), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: The Clearing House (RTP)
provider_slug: the-clearing-house
slug: the-clearing-house-domain-security
source_filename: the-clearing-house-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.theclearinghouse.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 23:59:59 2026 GMT\n  hsts: true\ndomains:\n- domain: theclearinghouse.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-clearing-house/refs/heads/main/security/the-clearing-house-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- United States
- Real-Time Payments
- Instant Payments
- ISO 20022
- Account-to-Account
- Payment Rails
- Scheme Operator
- Request for Payment
---
