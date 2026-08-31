---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: rxredefined.com
  spf: true
hosts:
- cert_expires: Feb 19 23:59:59 2027 GMT
  host: rxredefined.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 21 17:20:26 2026 GMT
  host: app.rxredefined.com
  hsts: false
  https: true
  note: Customer-only application host (Aptible-hosted). Probed manually on 2026-08-26; the automated pass only reads hosts named by apis.yml Website/baseURL.
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Rx Redefined Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rx Redefined, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Rx Redefined
provider_slug: rx-redefined
slug: rx-redefined-domain-security
source_filename: rx-redefined-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rxredefined.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 19 23:59:59 2027 GMT\n  hsts: false\n- host: app.rxredefined.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 21 17:20:26 2026 GMT\n  hsts: false\n  note: >-\n    Customer-only application host (Aptible-hosted). Probed manually on 2026-08-26; the\n    automated pass only reads hosts named by apis.yml Website/baseURL.\ndomains:\n- domain: rxredefined.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rx-redefined/refs/heads/main/security/rx-redefined-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthcare
- Medical Supplies
- DMEPOS
- Durable Medical Equipment
- Compliance
- HIPAA
- Revenue Cycle Management
- Supply Chain
- Physicians
- Clinical
---
