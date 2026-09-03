---
api_specs:
- filename: usm-repository-oai-pmh-openapi.yml
  format: yaml
  label: USM Repository OAI-PMH
  slug: eprints-oai
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usm/refs/heads/main/openapi/usm-repository-oai-pmh-openapi.yml
- filename: usm-repository-eprints-rest-openapi.yml
  format: yaml
  label: USM Repository EPrints REST and Export
  slug: eprints-rest
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usm/refs/heads/main/openapi/usm-repository-eprints-rest-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: usm.my
  spf: true
hosts:
- cert_expires: Aug 25 07:01:10 2026 GMT
  host: www.usm.my
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 25 07:01:10 2026 GMT
  host: eprints.usm.my
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug 25 07:01:10 2026 GMT
  host: api.usm.my
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Usm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Universiti Sains Malaysia, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Universiti Sains Malaysia
provider_slug: usm
slug: usm-domain-security
source_filename: usm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.usm.my\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 07:01:10 2026 GMT\n  hsts: false\n- host: eprints.usm.my\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 25 07:01:10 2026 GMT\n  hsts: false\n- host: api.usm.my\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 25 07:01:10 2026 GMT\n  hsts: false\ndomains:\n- domain: usm.my\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/usm/refs/heads/main/security/usm-domain-security.yml
summary_line: TLSv1.3
tags:
- University
- Higher Education
- Education
- Public Research University
- Malaysia
- Southeast Asia
- Research
- Open Access
- Institutional Repository
- OAI-PMH
- EPrints
- Identity Federation
- Shibboleth
- SAML
- Crossref
---
