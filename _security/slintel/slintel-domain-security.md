---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: slintel.com
  spf: true
hosts:
- cert_expires: Aug 29 00:39:05 2026 GMT
  host: www.slintel.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Slintel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Slintel, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Slintel
provider_slug: slintel
slug: slintel-domain-security
source_filename: slintel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.slintel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 00:39:05 2026 GMT\n  hsts: false\ndomains:\n- domain: slintel.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/slintel/refs/heads/main/security/slintel-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Company
- Automation
- Sales Intelligence
- Market Intelligence
- Data Enrichment
- Firmographics
- Buying Intent
- B2B
---
