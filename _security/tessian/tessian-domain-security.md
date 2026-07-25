---
api_specs:
- filename: tessian-anomalies-api-openapi.yml
  format: yaml
  label: Tessian Anomalies API
  slug: tessian-anomalies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tessian/refs/heads/main/openapi/tessian-anomalies-api-openapi.yml
- filename: tessian-audits-api-openapi.yml
  format: yaml
  label: Tessian Audits API
  slug: tessian-audits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tessian/refs/heads/main/openapi/tessian-audits-api-openapi.yml
- filename: tessian-beta-endpoints-api-openapi.yml
  format: yaml
  label: Tessian Beta Endpoints API
  slug: tessian-beta-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tessian/refs/heads/main/openapi/tessian-beta-endpoints-api-openapi.yml
- filename: tessian-deprecated-api-openapi.yml
  format: yaml
  label: Tessian Deprecated API
  slug: tessian-deprecated-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tessian/refs/heads/main/openapi/tessian-deprecated-api-openapi.yml
- filename: tessian-endpoints-api-openapi.yml
  format: yaml
  label: Tessian Endpoints API
  slug: tessian-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tessian/refs/heads/main/openapi/tessian-endpoints-api-openapi.yml
- filename: tessian-events-api-openapi.yml
  format: yaml
  label: Tessian Events API
  slug: tessian-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tessian/refs/heads/main/openapi/tessian-events-api-openapi.yml
- filename: tessian-groups-api-openapi.yml
  format: yaml
  label: Tessian Groups API
  slug: tessian-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tessian/refs/heads/main/openapi/tessian-groups-api-openapi.yml
- filename: tessian-monitoring-api-openapi.yml
  format: yaml
  label: Tessian Monitoring API
  slug: tessian-monitoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tessian/refs/heads/main/openapi/tessian-monitoring-api-openapi.yml
- filename: tessian-risk-api-openapi.yml
  format: yaml
  label: Tessian Risk API
  slug: tessian-risk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tessian/refs/heads/main/openapi/tessian-risk-api-openapi.yml
- filename: tessian-triggers-api-openapi.yml
  format: yaml
  label: Tessian Triggers API
  slug: tessian-triggers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tessian/refs/heads/main/openapi/tessian-triggers-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tessian.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tessian-platform.com
  spf: false
hosts:
- cert_expires: Nov 26 23:59:59 2026 GMT
  host: www.tessian.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 26 23:59:59 2026 GMT
  host: your-domain.tessian-platform.com
  hsts: true
  hsts_max_age: 7776000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 22 23:59:59 2027 GMT
  host: your-domain.tessian-app.com
  hsts: true
  hsts_max_age: 7776000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tessian Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tessian, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Tessian
provider_slug: tessian
slug: tessian-domain-security
source_filename: tessian-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tessian.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: your-domain.tessian-platform.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 7776000\n- host: your-domain.tessian-app.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 7776000\ndomains:\n- domain: tessian.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: tessian-platform.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tessian/refs/heads/main/security/tessian-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Enterprise
- Email Security
- Cybersecurity
- Data Loss Prevention
- SIEM
- Security
- Phishing
---
