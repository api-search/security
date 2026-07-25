---
api_specs:
- filename: xbow-assessments-api-openapi.yml
  format: yaml
  label: Xbow Assessments API
  slug: xbow-assessments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xbow/refs/heads/main/openapi/xbow-assessments-api-openapi.yml
- filename: xbow-assets-api-openapi.yml
  format: yaml
  label: Xbow Assets API
  slug: xbow-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xbow/refs/heads/main/openapi/xbow-assets-api-openapi.yml
- filename: xbow-findings-api-openapi.yml
  format: yaml
  label: Xbow Findings API
  slug: xbow-findings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xbow/refs/heads/main/openapi/xbow-findings-api-openapi.yml
- filename: xbow-lightspeed-api-openapi.yml
  format: yaml
  label: Xbow Lightspeed API
  slug: xbow-lightspeed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xbow/refs/heads/main/openapi/xbow-lightspeed-api-openapi.yml
- filename: xbow-meta-api-openapi.yml
  format: yaml
  label: Xbow Meta API
  slug: xbow-meta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xbow/refs/heads/main/openapi/xbow-meta-api-openapi.yml
- filename: xbow-organizations-api-openapi.yml
  format: yaml
  label: Xbow Organizations API
  slug: xbow-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xbow/refs/heads/main/openapi/xbow-organizations-api-openapi.yml
- filename: xbow-reports-api-openapi.yml
  format: yaml
  label: Xbow Reports API
  slug: xbow-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xbow/refs/heads/main/openapi/xbow-reports-api-openapi.yml
- filename: xbow-resources-api-openapi.yml
  format: yaml
  label: Xbow Resources API
  slug: xbow-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xbow/refs/heads/main/openapi/xbow-resources-api-openapi.yml
- filename: xbow-webhooks-api-openapi.yml
  format: yaml
  label: Xbow Webhooks API
  slug: xbow-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xbow/refs/heads/main/openapi/xbow-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: xbow.com
  spf: true
hosts:
- cert_expires: Sep 22 15:22:40 2026 GMT
  host: xbow.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 25 17:21:21 2026 GMT
  host: docs.xbow.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 14:15:26 2026 GMT
  host: console.xbow.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Xbow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Xbow, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Xbow
provider_slug: xbow
slug: xbow-domain-security
source_filename: xbow-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: xbow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 15:22:40 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.xbow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 17:21:21 2026 GMT\n  hsts: false\n- host: console.xbow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 14:15:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: xbow.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xbow/refs/heads/main/security/xbow-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Security
- Penetration Testing
- Offensive Security
- Artificial Intelligence
- Vulnerability Management
- Cybersecurity
- Application Security
---
