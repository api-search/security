---
api_specs:
- filename: chaoss-complexity-api-openapi.yml
  format: yaml
  label: CHAOSS Complexity API
  slug: chaoss-complexity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chaoss/refs/heads/main/openapi/chaoss-complexity-api-openapi.yml
- filename: chaoss-dei-badging-api-openapi.yml
  format: yaml
  label: CHAOSS DEI Badging API
  slug: chaoss-dei-badging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chaoss/refs/heads/main/openapi/chaoss-dei-badging-api-openapi.yml
- filename: chaoss-evolution-api-openapi.yml
  format: yaml
  label: CHAOSS Evolution API
  slug: chaoss-evolution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chaoss/refs/heads/main/openapi/chaoss-evolution-api-openapi.yml
- filename: chaoss-experimental-api-openapi.yml
  format: yaml
  label: CHAOSS Experimental API
  slug: chaoss-experimental-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chaoss/refs/heads/main/openapi/chaoss-experimental-api-openapi.yml
- filename: chaoss-login-api-openapi.yml
  format: yaml
  label: CHAOSS Login API
  slug: chaoss-login-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chaoss/refs/heads/main/openapi/chaoss-login-api-openapi.yml
- filename: chaoss-risk-api-openapi.yml
  format: yaml
  label: CHAOSS Risk API
  slug: chaoss-risk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chaoss/refs/heads/main/openapi/chaoss-risk-api-openapi.yml
- filename: chaoss-utility-api-openapi.yml
  format: yaml
  label: CHAOSS Utility API
  slug: chaoss-utility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chaoss/refs/heads/main/openapi/chaoss-utility-api-openapi.yml
- filename: chaoss-value-api-openapi.yml
  format: yaml
  label: CHAOSS Value API
  slug: chaoss-value-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chaoss/refs/heads/main/openapi/chaoss-value-api-openapi.yml
- filename: chaoss-visualizations-api-openapi.yml
  format: yaml
  label: CHAOSS Visualizations API
  slug: chaoss-visualizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chaoss/refs/heads/main/openapi/chaoss-visualizations-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: chaoss.community
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: collectoss.org
  spf: false
hosts:
- cert_expires: Dec  4 06:35:39 2026 GMT
  host: chaoss.community
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 22 12:59:38 2026 GMT
  host: docs.collectoss.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  3 15:44:43 2026 GMT
  host: www.chaoss.community
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Chaoss Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CHAOSS, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: CHAOSS
provider_slug: chaoss
slug: chaoss-domain-security
source_filename: chaoss-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: chaoss.community\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 06:35:39 2026 GMT\n  hsts: false\n- host: docs.collectoss.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 12:59:38 2026 GMT\n  hsts: false\n- host: www.chaoss.community\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 15:44:43 2026 GMT\n  hsts: false\ndomains:\n- domain: chaoss.community\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: collectoss.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chaoss/refs/heads/main/security/chaoss-domain-security.yml
summary_line: TLSv1.3
tags:
- Analytics
- Community Health
- DEI
- Linux Foundation
- Metrics
- Observability
- Open Source
- Risk Management
- Sustainability
---
