---
api_specs:
- filename: bureau-of-reclamation-openapi.yml
  format: yaml
  label: Reclamation Information Sharing Environment (RISE) API
  slug: reclamation-information-sharing-environment-rise
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bureau-of-reclamation/refs/heads/main/openapi/bureau-of-reclamation-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: usbr.gov
  spf: true
hosts:
- cert_expires: Jan 26 23:59:59 2027 GMT
  host: www.usbr.gov
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan 26 23:59:59 2027 GMT
  host: data.usbr.gov
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Bureau Of Reclamation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bureau of Reclamation, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Bureau of Reclamation
provider_slug: bureau-of-reclamation
slug: bureau-of-reclamation-domain-security
source_filename: bureau-of-reclamation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.usbr.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 26 23:59:59 2027 GMT\n  hsts: null\n- host: data.usbr.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 26 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: usbr.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bureau-of-reclamation/refs/heads/main/security/bureau-of-reclamation-domain-security.yml
summary_line: TLSv1.2 · DNSSEC · DMARC
tags:
- Energy
- Federal Government
- Infrastructure
- Water
- Hydrology
- Reservoirs
---
