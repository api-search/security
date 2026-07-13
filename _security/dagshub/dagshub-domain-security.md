---
api_specs:
- filename: dagshub-openapi.yml
  format: yaml
  label: DagsHub REST API
  slug: dagshub-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dagshub/refs/heads/main/openapi/dagshub-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: dagshub.com
  spf: true
hosts:
- cert_expires: Sep 11 23:59:59 2026 GMT
  host: dagshub.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dagshub Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DagsHub, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: DagsHub
provider_slug: dagshub
slug: dagshub-domain-security
source_filename: dagshub-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dagshub.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: dagshub.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dagshub/refs/heads/main/security/dagshub-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- ML
- MLOps
- Data Versioning
- Git
- MLflow
---
