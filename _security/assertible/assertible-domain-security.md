---
api_specs:
- filename: assertible-openapi.yml
  format: yaml
  label: Assertible API
  slug: assertible-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/assertible/refs/heads/main/openapi/assertible-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: assertible.com
  spf: true
hosts:
- cert_expires: Jan 17 23:59:59 2027 GMT
  host: assertible.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- host: api.assertible.com
  https: false
kind: domain-security
layout: security
method: probed
name: Assertible Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Assertible, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Assertible
provider_slug: assertible
slug: assertible-domain-security
source_filename: assertible-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: assertible.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 17 23:59:59 2027 GMT\n  hsts: false\n- host: api.assertible.com\n  https: false\ndomains:\n- domain: assertible.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/assertible/refs/heads/main/security/assertible-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- API Testing
- Monitoring
- Quality Assurance
- Testing
- CI/CD
---
