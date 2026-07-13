---
api_specs:
- filename: okta-openapi-original.yml
  format: yaml
  label: Okta API
  slug: okta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/okta/refs/heads/main/openapi/okta-openapi-original.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issuewild "digicert.com"
  - 0 issuewild "globalsign.com"
  - 0 iodef "mailto:ops@okta.com"
  - 0 iodef "mailto:security-alert@okta.com"
  - 0 issue "amazonaws.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: okta.com
  spf: true
hosts:
- cert_expires: Sep 12 23:59:59 2026 GMT
  host: www.okta.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 23:59:59 2026 GMT
  host: developer.okta.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 15 23:59:59 2027 GMT
  host: your-subdomain.okta.com
  hsts: true
  hsts_max_age: 315360000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Okta Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Okta, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Okta
provider_slug: okta
slug: okta-domain-security
source_filename: okta-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.okta.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.okta.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 23:59:59 2026 GMT\n  hsts: false\n- host: your-subdomain.okta.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 15 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 315360000\ndomains:\n- domain: okta.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"globalsign.com\"\n  - 0 iodef \"mailto:ops@okta.com\"\n  - 0 iodef \"mailto:security-alert@okta.com\"\n  - 0 issue \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/okta/refs/heads/main/security/okta-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Identity
- Workforce Identity
- Customer Identity
- Authentication
- Authorization
- Single Sign-On
- Multi-Factor Authentication
- Identity Governance
- Privileged Access
- AI Agents
- Cross-App Access
- MCP
- Platform
---
