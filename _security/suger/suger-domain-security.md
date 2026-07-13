---
api_specs:
- filename: suger-openapi.yml
  format: yaml
  label: Suger API
  slug: suger
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/suger/refs/heads/main/openapi/suger-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: suger.io
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: suger.cloud
  spf: false
hosts:
- cert_expires: Sep 27 03:55:27 2026 GMT
  host: www.suger.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 18 23:59:59 2027 GMT
  host: api.suger.cloud
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Suger Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Suger, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Suger
provider_slug: suger
slug: suger-domain-security
source_filename: suger-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.suger.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 03:55:27 2026 GMT\n  hsts: false\n- host: api.suger.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 18 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: suger.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: suger.cloud\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/suger/refs/heads/main/security/suger-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Cloud Marketplace
- GTM
- SaaS
- Billing
- Entitlement
- Revenue
- Co-Sell
---
