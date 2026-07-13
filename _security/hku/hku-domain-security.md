---
api_specs:
- filename: hku-datahub.yaml
  format: yaml
  label: HKU DataHub (Figshare)
  slug: datahub
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hku/refs/heads/main/openapi/hku-datahub.yaml
description: ''
domains:
- caa:
  - 0 issue "ecert.gov.hk"
  - 0 issue "letsencrypt.org"
  - 0 issue "comodoca.com"
  - 0 issuewild "digicert.com"
  - 0 issue "godaddy.com"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hku.hk
  spf: true
hosts:
- cert_expires: Dec 10 23:59:59 2026 GMT
  host: www.hku.hk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 10 23:59:59 2026 GMT
  host: developer.hku.hk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 21 23:59:59 2026 GMT
  host: datahub.hku.hk
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hku Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of Hong Kong, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: University of Hong Kong
provider_slug: hku
slug: hku-domain-security
source_filename: hku-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hku.hk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.hku.hk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: datahub.hku.hk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: hku.hk\n  dnssec: false\n  caa:\n  - 0 issue \"ecert.gov.hk\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"comodoca.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hku/refs/heads/main/security/hku-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Research Data
- Open Access
- Hong Kong
---
