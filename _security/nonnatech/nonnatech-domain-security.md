---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: nonnatech.com
  spf: true
hosts:
- cert_expires: Sep 28 16:02:55 2026 GMT
  host: nonnatech.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nonnatech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nonnatech, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Nonnatech
provider_slug: nonnatech
slug: nonnatech-domain-security
source_filename: nonnatech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nonnatech.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 16:02:55 2026 GMT\n  hsts: false\ndomains:\n- domain: nonnatech.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nonnatech/refs/heads/main/security/nonnatech-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Healthcare
- Remote Patient Monitoring
- Digital Health
- Telehealth
- HIPAA
- Population Health
- Chronic Care
---
