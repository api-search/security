---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: aisin.com
  spf: false
hosts:
- cert_expires: Dec 12 23:59:59 2026 GMT
  host: www.aisin.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aisin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aisin, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Aisin
provider_slug: aisin
slug: aisin-domain-security
source_filename: aisin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aisin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: aisin.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aisin/refs/heads/main/security/aisin-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Automotive
- Tier 1 Supplier
- Transmissions
- Drivetrain
- Toyota Group
---
