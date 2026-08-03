---
api_specs:
- filename: unqork-customer-api-openapi.yml
  format: yaml
  label: Unqork Customer API
  slug: unqork-customer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unqork/refs/heads/main/openapi/unqork-customer-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: unqork.com
  spf: true
- caa:
  - 0 issue "godaddy.com"
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  - 0 issue "amazontrust.com"
  - 0 issue "csc.com"
  - 0 issue "cscglobal.com"
  dmarc: false
  dnssec: false
  domain: unqork.io
  spf: false
hosts:
- cert_expires: Sep 27 20:53:23 2026 GMT
  host: unqork.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 28 23:59:59 2026 GMT
  host: developers.unqork.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 10 23:59:59 2027 GMT
  host: training.unqork.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Unqork Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Unqork, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Unqork
provider_slug: unqork
slug: unqork-domain-security
source_filename: unqork-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: unqork.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 20:53:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.unqork.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 23:59:59 2026 GMT\n  hsts: false\n- host: training.unqork.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: unqork.com\n  dnssec: true\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: unqork.io\n  dnssec: false\n  caa:\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"csc.com\"\n  - 0 issue \"cscglobal.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unqork/refs/heads/main/security/unqork-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- No-Code
- Low-Code
- Application Development
- Enterprise Software
- Platform as a Service
- Workflow
- Financial Services
- Insurance
- Government
- Application Modernization
---
