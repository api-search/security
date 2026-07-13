---
api_specs:
- filename: 34965-8158-rest-api.html
  format: yaml
  label: Checkmarx SAST API
  slug: checkmarx-sast-api
  spec_type: OpenAPI
  url: https://checkmarx.com/resource/documents/en/34965-8158-rest-api.html
- filename: checkmarx-sca-openapi.yml
  format: yaml
  label: Checkmarx SCA API
  slug: checkmarx-sca-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkmarx/refs/heads/main/openapi/checkmarx-sca-openapi.yml
- filename: checkmarx-one-openapi.yml
  format: yaml
  label: Checkmarx One API
  slug: checkmarx-one-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkmarx/refs/heads/main/openapi/checkmarx-one-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: checkmarx.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: your-checkmarx-instance.com
  spf: false
hosts:
- cert_expires: Sep 17 16:25:35 2026 GMT
  host: www.checkmarx.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 15 11:28:19 2026 GMT
  host: checkmarx.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: your-checkmarx-instance.com
  https: false
kind: domain-security
layout: security
method: probed
name: Checkmarx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Checkmarx, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Checkmarx
provider_slug: checkmarx
slug: checkmarx-domain-security
source_filename: checkmarx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.checkmarx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 16:25:35 2026 GMT\n  hsts: false\n- host: checkmarx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 11:28:19 2026 GMT\n  hsts: false\n- host: your-checkmarx-instance.com\n  https: false\ndomains:\n- domain: checkmarx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: your-checkmarx-instance.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/checkmarx/refs/heads/main/security/checkmarx-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Application Security
- Code Analysis
- DevSecOps
- SAST
- Security Testing
- Vulnerability Scanning
---
