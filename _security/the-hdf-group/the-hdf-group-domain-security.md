---
api_specs:
- filename: hdfgroup-openapi.yaml
  format: yaml
  label: HSDS REST API
  slug: hsds-rest-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/the-hdf-group/openapi/hdfgroup-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hdfgroup.org
  spf: true
hosts:
- cert_expires: Dec 19 20:31:08 2026 GMT
  host: www.hdfgroup.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: The Hdf Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The HDF Group, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: The HDF Group
provider_slug: the-hdf-group
slug: the-hdf-group-domain-security
source_filename: the-hdf-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hdfgroup.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 20:31:08 2026 GMT\n  hsts: false\ndomains:\n- domain: hdfgroup.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/the-hdf-group/security/the-hdf-group-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Data Management
- Open Source
- Scientific Computing
- Nonprofit
---
