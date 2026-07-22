---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: fortu.co.uk
  spf: false
hosts:
- cert_expires: Sep 21 08:59:40 2026 GMT
  host: fortu.co.uk
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fortu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fortu, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Fortu
provider_slug: fortu
slug: fortu-domain-security
source_filename: fortu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fortu.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 08:59:40 2026 GMT\n  hsts: null\ndomains:\n- domain: fortu.co.uk\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fortu/refs/heads/main/security/fortu-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Fintech
- Private Banking
- Wealth Management
- Banking as a Service
- Payments
- Compliance
- Embedded Finance
---
