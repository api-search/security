---
api_specs:
- filename: digital-realty-openapi-generated.yml
  format: yaml
  label: Digital Realty API
  slug: digital-realty-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digital-realty/refs/heads/main/openapi/_ae-authored/digital-realty-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "digicert.com"
  - 0 issue "entrust.net"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: digitalrealty.com
  spf: true
hosts:
- cert_expires: Nov 22 01:32:42 2026 GMT
  host: www.digitalrealty.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Digital Realty Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Digital Realty, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Digital Realty
provider_slug: digital-realty
slug: digital-realty-domain-security
source_filename: digital-realty-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.digitalrealty.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 22 01:32:42 2026 GMT\n  hsts: false\ndomains:\n- domain: digitalrealty.com\n  dnssec: false\n  caa:\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"entrust.net\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/digital-realty/refs/heads/main/security/digital-realty-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- DataCenter
- Colocation
- Cloud
- Infrastructure
- Sustainability
---
