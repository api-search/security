---
api_specs:
- filename: uclouvain-dataverse-api.yaml
  format: yaml
  label: Open Data @ UCLouvain Dataverse API
  slug: dataverse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uclouvain/refs/heads/main/openapi/uclouvain-dataverse-api.yaml
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
- Education
- Higher Education
- University
- Open Data
- Open Science
- Research Data
- Library
- OAI-PMH
- Belgium
---
