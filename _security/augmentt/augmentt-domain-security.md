---
api_specs:
- filename: augmentt-customers-api-openapi.yml
  format: yaml
  label: Augmentt Customers API
  slug: augmentt-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/augmentt/refs/heads/main/openapi/augmentt-customers-api-openapi.yml
- filename: augmentt-licensing-api-openapi.yml
  format: yaml
  label: Augmentt Licensing API
  slug: augmentt-licensing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/augmentt/refs/heads/main/openapi/augmentt-licensing-api-openapi.yml
- filename: augmentt-security-reports-api-openapi.yml
  format: yaml
  label: Augmentt Security Reports API
  slug: augmentt-security-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/augmentt/refs/heads/main/openapi/augmentt-security-reports-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "awstrust.com"
  - 0 iodef "mailto:security@augmentt.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: augmentt.com
  spf: true
hosts:
- cert_expires: Dec 11 20:59:21 2026 GMT
  host: www.augmentt.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 11 23:59:59 2027 GMT
  host: api.augmentt.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 11 23:59:59 2027 GMT
  host: api.eu.augmentt.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Augmentt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Augmentt, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Augmentt
provider_slug: augmentt
slug: augmentt-domain-security
source_filename: augmentt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.augmentt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 20:59:21 2026 GMT\n  hsts: false\n- host: api.augmentt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 23:59:59 2027 GMT\n  hsts: null\n- host: api.eu.augmentt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 11 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: augmentt.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"awstrust.com\"\n  - 0 iodef \"mailto:security@augmentt.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/augmentt/refs/heads/main/security/augmentt-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- MSP
- Microsoft-365
- SaaS Management
- SaaS Security
- Shadow IT
- Security Posture
- Compliance
- License Management
- Multi-Tenant
- Reporting
---
