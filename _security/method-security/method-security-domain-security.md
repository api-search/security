---
api_specs:
- filename: method-security-audit-api-openapi.yml
  format: yaml
  label: Method Security audit API
  slug: method-security-audit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/method-security/refs/heads/main/openapi/method-security-audit-api-openapi.yml
- filename: method-security-auth-api-openapi.yml
  format: yaml
  label: Method Security auth API
  slug: method-security-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/method-security/refs/heads/main/openapi/method-security-auth-api-openapi.yml
- filename: method-security-blueprints-api-openapi.yml
  format: yaml
  label: Method Security blueprints API
  slug: method-security-blueprints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/method-security/refs/heads/main/openapi/method-security-blueprints-api-openapi.yml
- filename: method-security-environments-api-openapi.yml
  format: yaml
  label: Method Security environments API
  slug: method-security-environments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/method-security/refs/heads/main/openapi/method-security-environments-api-openapi.yml
- filename: method-security-issues-api-openapi.yml
  format: yaml
  label: Method Security issues API
  slug: method-security-issues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/method-security/refs/heads/main/openapi/method-security-issues-api-openapi.yml
- filename: method-security-reports-api-openapi.yml
  format: yaml
  label: Method Security reports API
  slug: method-security-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/method-security/refs/heads/main/openapi/method-security-reports-api-openapi.yml
- filename: method-security-signals-api-openapi.yml
  format: yaml
  label: Method Security signals API
  slug: method-security-signals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/method-security/refs/heads/main/openapi/method-security-signals-api-openapi.yml
- filename: method-security-skills-api-openapi.yml
  format: yaml
  label: Method Security skills API
  slug: method-security-skills-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/method-security/refs/heads/main/openapi/method-security-skills-api-openapi.yml
- filename: method-security-system-api-openapi.yml
  format: yaml
  label: Method Security system API
  slug: method-security-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/method-security/refs/heads/main/openapi/method-security-system-api-openapi.yml
- filename: method-security-targets-api-openapi.yml
  format: yaml
  label: Method Security targets API
  slug: method-security-targets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/method-security/refs/heads/main/openapi/method-security-targets-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: method.security
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: method.delivery
  spf: false
hosts:
- cert_expires: Sep 21 21:38:53 2026 GMT
  host: method.security
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 21:26:35 2026 GMT
  host: docs.method.security
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: your-instance.method.delivery
  https: false
kind: domain-security
layout: security
method: probed
name: Method Security Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Method Security, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Method Security
provider_slug: method-security
slug: method-security-domain-security
source_filename: method-security-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: method.security\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 21:38:53 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.method.security\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 21:26:35 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: your-instance.method.delivery\n  https: false\ndomains:\n- domain: method.security\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: method.delivery\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/method-security/refs/heads/main/security/method-security-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Security
- Cybersecurity
- Offensive Security
- Exposure Management
- Attack Surface Management
- Vulnerability Management
- Red Team
- AI Agents
- Government
---
