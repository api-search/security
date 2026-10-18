---
api_specs:
- filename: cumulio-authorize-api-openapi.yml
  format: yaml
  label: Cumulio Authorize API
  slug: cumulio-authorize-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cumulio/refs/heads/main/openapi/cumulio-authorize-api-openapi.yml
- filename: cumulio-datasets-api-openapi.yml
  format: yaml
  label: Cumulio Datasets API
  slug: cumulio-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cumulio/refs/heads/main/openapi/cumulio-datasets-api-openapi.yml
- filename: cumulio-exchange-api-openapi.yml
  format: yaml
  label: Cumulio Exchange API
  slug: cumulio-exchange-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cumulio/refs/heads/main/openapi/cumulio-exchange-api-openapi.yml
- filename: cumulio-query-api-openapi.yml
  format: yaml
  label: Cumulio Query API
  slug: cumulio-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cumulio/refs/heads/main/openapi/cumulio-query-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: luzmo.com
  spf: true
hosts:
- cert_expires: Jan  1 23:59:59 2027 GMT
  host: www.luzmo.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cumulio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cumulio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cumulio
provider_slug: cumulio
slug: cumulio-domain-security
source_filename: cumulio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.luzmo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: luzmo.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cumulio/refs/heads/main/security/cumulio-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
