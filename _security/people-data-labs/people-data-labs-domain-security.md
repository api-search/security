---
api_specs:
- filename: people-data-labs-openapi.yml
  format: yaml
  label: People Data Labs API
  slug: people-data-labs
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/people-data-labs/refs/heads/main/openapi/people-data-labs-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: peopledatalabs.com
  spf: true
hosts:
- cert_expires: Aug 26 14:44:04 2026 GMT
  host: www.peopledatalabs.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 28 23:59:59 2027 GMT
  host: api.peopledatalabs.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: People Data Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for People Data Labs, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: People Data Labs
provider_slug: people-data-labs
slug: people-data-labs-domain-security
source_filename: people-data-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.peopledatalabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 14:44:04 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.peopledatalabs.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 28 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: peopledatalabs.com\n  dnssec: true\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/people-data-labs/refs/heads/main/security/people-data-labs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- B2B
- Identity Resolution
- People Data
---
