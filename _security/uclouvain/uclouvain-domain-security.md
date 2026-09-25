---
api_specs:
- filename: uclouvain-instances-api-openapi.yml
  format: yaml
  label: UCLouvain Instances API
  slug: uclouvain-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uclouvain/refs/heads/main/openapi/uclouvain-instances-api-openapi.yml
- filename: uclouvain-jobs-api-openapi.yml
  format: yaml
  label: UCLouvain Jobs API
  slug: uclouvain-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uclouvain/refs/heads/main/openapi/uclouvain-jobs-api-openapi.yml
- filename: uclouvain-logs-api-openapi.yml
  format: yaml
  label: UCLouvain Logs API
  slug: uclouvain-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uclouvain/refs/heads/main/openapi/uclouvain-logs-api-openapi.yml
- filename: uclouvain-networking-api-openapi.yml
  format: yaml
  label: UCLouvain Networking API
  slug: uclouvain-networking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uclouvain/refs/heads/main/openapi/uclouvain-networking-api-openapi.yml
- filename: uclouvain-other-api-openapi.yml
  format: yaml
  label: UCLouvain Other API
  slug: uclouvain-other-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uclouvain/refs/heads/main/openapi/uclouvain-other-api-openapi.yml
- filename: uclouvain-patients-api-openapi.yml
  format: yaml
  label: UCLouvain Patients API
  slug: uclouvain-patients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uclouvain/refs/heads/main/openapi/uclouvain-patients-api-openapi.yml
- filename: uclouvain-series-api-openapi.yml
  format: yaml
  label: UCLouvain Series API
  slug: uclouvain-series-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uclouvain/refs/heads/main/openapi/uclouvain-series-api-openapi.yml
- filename: uclouvain-studies-api-openapi.yml
  format: yaml
  label: UCLouvain Studies API
  slug: uclouvain-studies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uclouvain/refs/heads/main/openapi/uclouvain-studies-api-openapi.yml
- filename: uclouvain-system-api-openapi.yml
  format: yaml
  label: UCLouvain System API
  slug: uclouvain-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uclouvain/refs/heads/main/openapi/uclouvain-system-api-openapi.yml
- filename: uclouvain-tracking-changes-api-openapi.yml
  format: yaml
  label: UCLouvain Tracking changes API
  slug: uclouvain-tracking-changes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uclouvain/refs/heads/main/openapi/uclouvain-tracking-changes-api-openapi.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:abuse@uclouvain.be"
  - 0 issue "amazontrust.com"
  - 0 issue "harica.gr"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: uclouvain.be
  spf: true
hosts:
- cert_expires: Jan 22 09:56:53 2027 GMT
  host: uclouvain.be
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 25 15:36:25 2026 GMT
  host: dataverse.uclouvain.be
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: dial.uclouvain.be
  https: false
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Uclouvain Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for UCLouvain, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: UCLouvain
provider_slug: uclouvain
slug: uclouvain-domain-security
source_filename: uclouvain-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: uclouvain.be\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 09:56:53 2027 GMT\n  hsts: null\n- host: dataverse.uclouvain.be\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 15:36:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: dial.uclouvain.be\n  https: false\ndomains:\n- domain: uclouvain.be\n  dnssec: true\n  caa:\n  - 0 iodef \"mailto:abuse@uclouvain.be\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"harica.gr\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uclouvain/refs/heads/main/security/uclouvain-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- University
- Higher Education
- Education
- Belgium
- Private Research University
- Open Data
- Research Data
- Open Science
- Institutional Repository
- OAI-PMH
- Identity Federation
- Open Source
- Medical Imaging
- Library
---
