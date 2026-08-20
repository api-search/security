---
api_specs:
- filename: kyoto-oai-pmh-api-openapi.yml
  format: yaml
  label: KURENAI OAI-PMH API
  slug: kyoto-oai-pmh-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kyoto/refs/heads/main/openapi/kyoto-oai-pmh-api-openapi.yml
- filename: kyoto-rest-api-openapi.yml
  format: yaml
  label: KURENAI DSpace REST API
  slug: kyoto-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kyoto/refs/heads/main/openapi/kyoto-rest-api-openapi.yml
- filename: kyoto-lms-api-openapi.yml
  format: yaml
  label: PandA Learning Support System API (Sakai Entity Broker + IMS LTI)
  slug: kyoto-lms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kyoto/refs/heads/main/openapi/kyoto-lms-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: kyoto-u.ac.jp
  spf: true
hosts:
- cert_expires: Jan  5 06:18:07 2027 GMT
  host: www.kyoto-u.ac.jp
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 18 02:23:04 2026 GMT
  host: repository.kulib.kyoto-u.ac.jp
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 25 00:43:34 2026 GMT
  host: www.iimc.kyoto-u.ac.jp
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Kyoto Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kyoto University, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Kyoto University
provider_slug: kyoto
slug: kyoto-domain-security
source_filename: kyoto-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kyoto-u.ac.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 06:18:07 2027 GMT\n  hsts: false\n- host: repository.kulib.kyoto-u.ac.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 02:23:04 2026 GMT\n  hsts: false\n- host: www.iimc.kyoto-u.ac.jp\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 25 00:43:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: kyoto-u.ac.jp\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kyoto/refs/heads/main/security/kyoto-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- University
- Higher Education
- Education
- Japan
- National University
- Research Repository
- Research Data
- Identity Federation
- Learning Management
- Open Access
- Research Computing
- Scholarly
---
