---
api_specs:
- filename: trellix-epo-saas-openapi.yml
  format: yaml
  label: Trellix ePO SaaS API
  slug: trellix-epo-saas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trellix/refs/heads/main/openapi/trellix-epo-saas-openapi.yml
- filename: trellix-edr-openapi.yml
  format: yaml
  label: Trellix EDR API
  slug: trellix-edr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trellix/refs/heads/main/openapi/trellix-edr-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: trellix.com
  spf: true
hosts:
- cert_expires: Sep 30 23:59:59 2026 GMT
  host: www.trellix.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 23:59:59 2026 GMT
  host: docs.trellix.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 24 23:59:59 2027 GMT
  host: api.manage.trellix.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Trellix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Trellix, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Trellix
provider_slug: trellix
slug: trellix-domain-security
source_filename: trellix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.trellix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 23:59:59 2026 GMT\n  hsts: null\n- host: docs.trellix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.manage.trellix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 24 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: trellix.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trellix/refs/heads/main/security/trellix-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cloud Security
- Cybersecurity
- Endpoint Security
- Threat Detection
- Threat Intelligence
- XDR
---
