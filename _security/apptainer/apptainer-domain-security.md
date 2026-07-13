---
api_specs:
- filename: apptainer-openapi.yaml
  format: yaml
  label: Apptainer API
  slug: apptainer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apptainer/refs/heads/main/openapi/apptainer-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: apptainer.org
  spf: true
hosts:
- cert_expires: Sep 20 03:19:21 2026 GMT
  host: apptainer.org
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
- host: api.apptainer.org
  https: false
kind: domain-security
layout: security
method: probed
name: Apptainer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apptainer, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Apptainer
provider_slug: apptainer
slug: apptainer-domain-security
source_filename: apptainer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: apptainer.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 03:19:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\n- host: api.apptainer.org\n  https: false\ndomains:\n- domain: apptainer.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apptainer/refs/heads/main/security/apptainer-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Containers
- HPC
- Scientific Computing
- Open Source
- Linux Foundation
---
