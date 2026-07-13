---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Kong Gateway Admin API
  slug: kong-gateway-admin-api
  spec_type: OpenAPI
  url: https://docs.konghq.com/gateway/latest/admin-api/
- filename: x-tyk-gateway.json
  format: json
  label: Tyk API Management API
  slug: tyk-api-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/TykTechnologies/tyk/master/apidef/oas/schema/x-tyk-gateway.json
- filename: api-spec.json
  format: json
  label: Grafana API
  slug: grafana-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/grafana/grafana/main/public/api-spec.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: konghq.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amazon.com
  spf: true
hosts:
- cert_expires: Oct  8 03:43:41 2026 GMT
  host: docs.konghq.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  8 23:59:59 2026 GMT
  host: docs.aws.amazon.com
  hsts: true
  hsts_max_age: 47304000
  https: true
  tls_version: TLSv1.3
- host: apigateway.amazonaws.com
  https: false
kind: domain-security
layout: security
method: probed
name: Test Rate Limit Check Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Test Rate Limit Check, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Test Rate Limit Check
provider_slug: test-rate-limit-check
slug: test-rate-limit-check-domain-security
source_filename: test-rate-limit-check-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.konghq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 03:43:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: apigateway.amazonaws.com\n  https: false\ndomains:\n- domain: konghq.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/test-rate-limit-check/refs/heads/main/security/test-rate-limit-check-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- API Governance
- API Management
- API Testing
- Performance Testing
- Rate Limiting
- Testing
---
