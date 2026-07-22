---
api_specs:
- filename: seqera-labs-platform-openapi.yml
  format: yaml
  label: Seqera Platform API
  slug: seqera-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seqera-labs/refs/heads/main/openapi/seqera-labs-platform-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog"
  - 0 iodef "mailto:devops@seqera.io"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: seqera.io
  spf: true
hosts:
- cert_expires: Sep 13 01:03:44 2026 GMT
  host: docs.seqera.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 11 23:59:59 2027 GMT
  host: api.cloud.seqera.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Seqera Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Seqera Labs, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Seqera Labs
provider_slug: seqera-labs
slug: seqera-labs-domain-security
source_filename: seqera-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.seqera.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 01:03:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.cloud.seqera.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 11 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: seqera.io\n  dnssec: false\n  caa:\n  - 0 issuewild \"pki.goog\"\n  - 0 iodef \"mailto:devops@seqera.io\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/seqera-labs/refs/heads/main/security/seqera-labs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Bioinformatics
- Workflow Orchestration
- Data Pipelines
- Scientific Computing
- Nextflow
- Cloud Compute
- Life Sciences
- Containers
- GA4GH
---
