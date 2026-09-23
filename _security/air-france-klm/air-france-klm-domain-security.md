---
api_specs:
- filename: air-france-klm-openapi-generated.yml
  format: yaml
  label: Air France-KLM API
  slug: air-france-klm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/air-france-klm/refs/heads/main/openapi/_ae-authored/air-france-klm-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: airfranceklm.com
  spf: true
hosts:
- cert_expires: Dec 16 14:37:30 2026 GMT
  host: airfranceklm.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Air France Klm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Air France-KLM, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Air France-KLM
provider_slug: air-france-klm
slug: air-france-klm-domain-security
source_filename: air-france-klm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: airfranceklm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 14:37:30 2026 GMT\n  hsts: null\ndomains:\n- domain: airfranceklm.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/air-france-klm/refs/heads/main/security/air-france-klm-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Aviation
- Travel
- Europe
- Sustainability
---
