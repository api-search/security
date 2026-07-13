---
api_specs:
- filename: account-info-openapi.yaml
  format: yaml
  label: UK Open Banking Read/Write API
  slug: uk-open-banking-readwrite-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/OpenBankingUK/read-write-api-specs/master/dist/openapi/account-info-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: openbanking.org.uk
  spf: true
hosts:
- cert_expires: Sep 24 23:59:59 2026 GMT
  host: www.openbanking.org.uk
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 23:59:59 2026 GMT
  host: standards.openbanking.org.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  9 23:59:59 2027 GMT
  host: directory.openbanking.org.uk
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Open Banking Uk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for UK Open Banking, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: UK Open Banking
provider_slug: open-banking-uk
slug: open-banking-uk-domain-security
source_filename: open-banking-uk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.openbanking.org.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: standards.openbanking.org.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: directory.openbanking.org.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: openbanking.org.uk\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/open-banking-uk/refs/heads/main/security/open-banking-uk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Open Banking
- Financial Services
- Payments
- Account Information
- PSD2
- UK
- Banking
- Fintech
- Regulated
---
