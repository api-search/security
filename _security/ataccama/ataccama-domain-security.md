---
api_specs:
- filename: ataccama-openapi-generated.yml
  format: yaml
  label: Ataccama API
  slug: ataccama-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ataccama/refs/heads/main/openapi/_ae-authored/ataccama-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issuewild "awstrust.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "sectigo.com"
  - 0 iodef "mailto:it@ataccama.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ataccama.com
  spf: true
hosts:
- cert_expires: Feb  9 23:59:59 2027 GMT
  host: www.ataccama.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ataccama Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ataccama, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Ataccama
provider_slug: ataccama
slug: ataccama-domain-security
source_filename: ataccama-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ataccama.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  9 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ataccama.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 iodef \"mailto:it@ataccama.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ataccama/refs/heads/main/security/ataccama-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Data Quality
- Data Governance
- AI
- Enterprise
- Platform
---
