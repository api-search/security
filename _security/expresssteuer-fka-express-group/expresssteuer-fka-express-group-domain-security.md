---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: expresssteuer.de
  spf: false
hosts:
- cert_expires: Sep 16 04:24:18 2026 GMT
  host: www.expresssteuer.de
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Expresssteuer Fka Express Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ExpressSteuer (fka Express Group), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: ExpressSteuer (fka Express Group)
provider_slug: expresssteuer-fka-express-group
slug: expresssteuer-fka-express-group-domain-security
source_filename: expresssteuer-fka-express-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.expresssteuer.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 04:24:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: expresssteuer.de\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/expresssteuer-fka-express-group/refs/heads/main/security/expresssteuer-fka-express-group-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Tax
- Taxation
- Fintech
- Financial Services
- Germany
- Tax Filing
- Consumer
---
