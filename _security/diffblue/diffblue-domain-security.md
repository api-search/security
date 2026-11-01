---
api_specs:
- filename: diffblue-diffblue-api-api-openapi.yml
  format: yaml
  label: Diffblue API
  slug: diffblue-api-2
  spec_type: OpenAPI
  url: https://artifacts.apis.io/diffblue/openapi/diffblue-diffblue-api-api-openapi.yml
- filename: diffblue-openapi-generated.yml
  format: yaml
  label: Diffblue API
  slug: diffblue-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/diffblue/openapi/_ae-authored/diffblue-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 iodef "mailto:it@diffblue.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: diffblue.com
  spf: true
hosts:
- cert_expires: Dec  7 17:23:06 2026 GMT
  host: www.diffblue.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Diffblue Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Diffblue, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Diffblue
provider_slug: diffblue
slug: diffblue-domain-security
source_filename: diffblue-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.diffblue.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 17:23:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: diffblue.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 iodef \"mailto:it@diffblue.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/diffblue/security/diffblue-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Testing
- Automation
- Enterprise
- Java
---
