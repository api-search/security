---
api_specs:
- filename: openapi.json
  format: json
  label: CoverWallet Insurance API
  slug: coverwallet-api
  spec_type: OpenAPI
  url: https://apidocs.aoncover.biz/swagger/public-api/openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: coverwallet.com
  spf: true
hosts:
- cert_expires: Dec 16 23:59:59 2026 GMT
  host: www.coverwallet.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 16 23:59:59 2026 GMT
  host: api.coverwallet.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Coverwallet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CoverWallet, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: CoverWallet
provider_slug: coverwallet
slug: coverwallet-domain-security
source_filename: coverwallet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.coverwallet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 23:59:59 2026 GMT\n  hsts: false\n- host: api.coverwallet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: coverwallet.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coverwallet/refs/heads/main/security/coverwallet-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Insurance
- Small Business
- Commercial Insurance
- General Liability
- BOP
- Professional Liability
- InsurTech
- Aon
---
