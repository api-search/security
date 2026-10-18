---
api_specs:
- filename: ebsco-content-api-openapi.yml
  format: yaml
  label: EBSCO Content API
  slug: ebsco-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ebsco/refs/heads/main/openapi/ebsco-content-api-openapi.yml
- filename: ebsco-publishers-api-openapi.yml
  format: yaml
  label: EBSCO Publishers API
  slug: ebsco-publishers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ebsco/refs/heads/main/openapi/ebsco-publishers-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: ebsco.com
  spf: true
hosts:
- cert_expires: Mar  6 19:02:18 2027 GMT
  host: www.ebsco.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ebsco Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EBSCO, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: EBSCO
provider_slug: ebsco
slug: ebsco-domain-security
source_filename: ebsco-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ebsco.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  6 19:02:18 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ebsco.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ebsco/refs/heads/main/security/ebsco-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Research
- Library
- Education
- Information
---
