---
api_specs:
- filename: federal-laboratory-consortium-for-technology-transfer-greenbook-openapi.yml
  format: yaml
  label: FLC Greenbook API
  slug: flc-greenbook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/federal-laboratory-consortium-for-technology-transfer/refs/heads/main/openapi/federal-laboratory-consortium-for-technology-transfer-greenbook-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: federallabs.org
  spf: true
hosts:
- cert_expires: Nov  8 02:05:58 2026 GMT
  host: www.federallabs.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  8 02:05:58 2026 GMT
  host: federallabs.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 19 19:02:14 2026 GMT
  host: api.federallabs.org
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Federal Laboratory Consortium For Technology Transfer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Federal Laboratory Consortium for Technology Transfer, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Federal Laboratory Consortium for Technology Transfer
provider_slug: federal-laboratory-consortium-for-technology-transfer
slug: federal-laboratory-consortium-for-technology-transfer-domain-security
source_filename: federal-laboratory-consortium-for-technology-transfer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.federallabs.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 02:05:58 2026 GMT\n  hsts: false\n- host: federallabs.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 02:05:58 2026 GMT\n  hsts: false\n- host: api.federallabs.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 19:02:14 2026 GMT\n  hsts: null\ndomains:\n- domain: federallabs.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/federal-laboratory-consortium-for-technology-transfer/refs/heads/main/security/federal-laboratory-consortium-for-technology-transfer-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Federal-Government
- Technology-Transfer
- Research
- Laboratories
- Government
- Innovation
- Search
---
