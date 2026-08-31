---
api_specs:
- filename: jitterbit-login-api-openapi.yml
  format: yaml
  label: Jitterbit Login API
  slug: jitterbit-login-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jitterbit/refs/heads/main/openapi/jitterbit-login-api-openapi.yml
- filename: jitterbit-operations-api-openapi.yml
  format: yaml
  label: Jitterbit Operations API
  slug: jitterbit-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jitterbit/refs/heads/main/openapi/jitterbit-operations-api-openapi.yml
- filename: jitterbit-projects-api-openapi.yml
  format: yaml
  label: Jitterbit Projects API
  slug: jitterbit-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jitterbit/refs/heads/main/openapi/jitterbit-projects-api-openapi.yml
- filename: jitterbit-schedules-api-openapi.yml
  format: yaml
  label: Jitterbit Schedules API
  slug: jitterbit-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jitterbit/refs/heads/main/openapi/jitterbit-schedules-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:operations@jitterbit.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: jitterbit.com
  spf: true
hosts:
- cert_expires: Dec 17 23:59:59 2026 GMT
  host: www.jitterbit.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 24 08:52:48 2026 GMT
  host: developer.jitterbit.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jitterbit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jitterbit, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Jitterbit
provider_slug: jitterbit
slug: jitterbit-domain-security
source_filename: jitterbit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.jitterbit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.jitterbit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 08:52:48 2026 GMT\n  hsts: false\ndomains:\n- domain: jitterbit.com\n  dnssec: true\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:operations@jitterbit.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jitterbit/refs/heads/main/security/jitterbit-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- API Management
- Automation
- Integration
- iPaaS
- EDI
- Low-Code
- Enterprise
- API Gateway
- Workflow-Automation
- Connectors
---
