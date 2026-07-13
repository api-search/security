---
api_specs:
- filename: snow-software-licenses-openapi.yml
  format: yaml
  label: Snow Atlas SAM Licenses API
  slug: snow-atlas-licenses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snow-software/refs/heads/main/openapi/snow-software-licenses-openapi.yml
- filename: snow-software-saas-applications-openapi.yml
  format: yaml
  label: Snow Atlas SaaS Applications API
  slug: snow-atlas-saas-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snow-software/refs/heads/main/openapi/snow-software-saas-applications-openapi.yml
- filename: snow-software-saas-subscriptions-openapi.yml
  format: yaml
  label: Snow Atlas SaaS Subscriptions API
  slug: snow-atlas-saas-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snow-software/refs/heads/main/openapi/snow-software-saas-subscriptions-openapi.yml
- filename: snow-software-computers-openapi.json
  format: json
  label: Snow Atlas SAM Computers API
  slug: snow-atlas-computers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snow-software/refs/heads/main/openapi/snow-software-computers-openapi.json
description: ''
domains:
- caa:
  - 0 iodef "mailto:dl.gl.infrastructureandoperations@snowsoftware.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: snowsoftware.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: flexera.com
  spf: true
hosts:
- cert_expires: Aug 28 23:05:05 2026 GMT
  host: www.snowsoftware.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec 23 23:59:59 2026 GMT
  host: docs.flexera.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Snow Software Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Snow Software, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Snow Software
provider_slug: snow-software
slug: snow-software-domain-security
source_filename: snow-software-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.snowsoftware.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 28 23:05:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.flexera.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: snowsoftware.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:dl.gl.infrastructureandoperations@snowsoftware.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: flexera.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/snow-software/refs/heads/main/security/snow-software-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Cloud License Management
- FinOps
- IT Asset Management
- SaaS Management
- Software Asset Management
---
