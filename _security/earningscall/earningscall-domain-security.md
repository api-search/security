---
api_specs:
- filename: earningscall-openapi-generated.yml
  format: yaml
  label: EarningsCall API
  slug: earningscall-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/earningscall/refs/heads/main/openapi/_ae-authored/earningscall-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: earningscall.biz
  spf: true
hosts:
- cert_expires: Feb 10 23:59:59 2027 GMT
  host: earningscall.biz
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Earningscall Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EarningsCall, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: EarningsCall
provider_slug: earningscall
slug: earningscall-domain-security
source_filename: earningscall-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: earningscall.biz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 10 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: earningscall.biz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/earningscall/refs/heads/main/security/earningscall-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Finance
- Data
- API
- Earnings
---
