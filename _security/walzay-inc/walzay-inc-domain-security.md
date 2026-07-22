---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: walzay.com
  spf: true
hosts:
- cert_expires: Aug 10 23:13:23 2026 GMT
  host: walzay.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Walzay Inc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Walzay Inc., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Walzay Inc.
provider_slug: walzay-inc
slug: walzay-inc-domain-security
source_filename: walzay-inc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: walzay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 10 23:13:23 2026 GMT\n  hsts: null\ndomains:\n- domain: walzay.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/walzay-inc/refs/heads/main/security/walzay-inc-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Recruitment
- Talent
- Hiring
- Marketplace
- Remote Work
---
