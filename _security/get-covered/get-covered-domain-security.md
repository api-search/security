---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: getcovered.io
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: getcoveredinsurance.com
  spf: true
hosts:
- cert_expires: Nov 24 23:59:59 2026 GMT
  host: www.getcovered.io
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec 24 23:59:59 2026 GMT
  host: api.getcoveredinsurance.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Get Covered Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Get Covered, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Get Covered
provider_slug: get-covered
slug: get-covered-domain-security
source_filename: get-covered-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.getcovered.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 24 23:59:59 2026 GMT\n  hsts: null\n- host: api.getcoveredinsurance.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: getcovered.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: getcoveredinsurance.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/get-covered/refs/heads/main/security/get-covered-domain-security.yml
summary_line: TLSv1.2 · DNSSEC · DMARC
tags:
- Company
- Insurance
- Insurtech
- Renters Insurance
- Property Management
- Real-Estate
- Compliance
- Risk Management
- Embedded Insurance
- Artificial Intelligence
---
