---
api_specs:
- filename: depayapp-com-openapi-generated.yml
  format: yaml
  label: Depay API
  slug: depayapp-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/depayapp-com/openapi/_ae-authored/depayapp-com-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issuewild "amazon.com"
  - 0 iodef "mailto:security@depay.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: depay.com
  spf: true
hosts:
- cert_expires: Mar  1 23:59:59 2027 GMT
  host: depay.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Depayapp Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Depay, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Depay
provider_slug: depayapp-com
slug: depayapp-com-domain-security
source_filename: depayapp-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: depay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  1 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: depay.com\n  dnssec: true\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 iodef \"mailto:security@depay.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/depayapp-com/security/depayapp-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Payments
- Crypto
- Web3
- FinTech
- API
---
