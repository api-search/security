---
api_specs:
- filename: zluri-api-openapi.yml
  format: yaml
  label: Zluri
  slug: zluri
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zluri/refs/heads/main/openapi/zluri-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazontrust.com"
  - 0 issue "ssl.com"
  - 0 issue "pki.goog"
  - 0 issue "amazonaws.com"
  - 0 issue "globalsign.com"
  - 0 issuewild "digicert.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: zluri.com
  spf: true
hosts:
- cert_expires: Sep 30 20:58:44 2026 GMT
  host: www.zluri.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 30 14:32:01 2026 GMT
  host: api-ext.zluri.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zluri Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zluri, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Zluri
provider_slug: zluri
slug: zluri-domain-security
source_filename: zluri-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.zluri.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 20:58:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-ext.zluri.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 14:32:01 2026 GMT\n  hsts: null\ndomains:\n- domain: zluri.com\n  dnssec: true\n  caa:\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issuewild \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zluri/refs/heads/main/security/zluri-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Access Management
- SaaS Management
---
