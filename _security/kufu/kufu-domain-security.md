---
api_specs:
- filename: kufu-smarthr-openapi.json
  format: json
  label: SmartHR API
  slug: smarthr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kufu/refs/heads/main/openapi/kufu-smarthr-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: smarthr.co.jp
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: smarthr.jp
  spf: true
hosts:
- cert_expires: Aug 26 17:16:13 2026 GMT
  host: smarthr.co.jp
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 16:05:33 2026 GMT
  host: app.smarthr.jp
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kufu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for KUFU, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: KUFU
provider_slug: kufu
slug: kufu-domain-security
source_filename: kufu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: smarthr.co.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 17:16:13 2026 GMT\n  hsts: false\n- host: app.smarthr.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 16:05:33 2026 GMT\n  hsts: false\ndomains:\n- domain: smarthr.co.jp\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: smarthr.jp\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kufu/refs/heads/main/security/kufu-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Human Resources
- HR Tech
- Payroll
- Employee Data
- SaaS
- Japan
- Onboarding
- Social Insurance
- Webhooks
---
