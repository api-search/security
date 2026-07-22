---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: servefirst.co.uk
  spf: true
hosts:
- cert_expires: Sep 29 16:23:36 2026 GMT
  host: servefirst.co.uk
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Serve First Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Serve First, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Serve First
provider_slug: serve-first
slug: serve-first-domain-security
source_filename: serve-first-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: servefirst.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 16:23:36 2026 GMT\n  hsts: false\ndomains:\n- domain: servefirst.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/serve-first/refs/heads/main/security/serve-first-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Customer Experience
- Customer Feedback
- Voice of the Customer
- Mystery Shopping
- Surveys
- Analytics
- Artificial Intelligence
- Retail
- Hospitality
---
