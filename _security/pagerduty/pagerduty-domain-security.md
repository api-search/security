---
api_specs:
- filename: pagerduty-openapi-original.yml
  format: yaml
  label: PagerDuty REST API
  slug: pagerduty-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagerduty/refs/heads/main/openapi/pagerduty-openapi-original.yml
- filename: pagerduty-events-asyncapi.yml
  format: yaml
  label: PagerDuty Events API
  slug: pagerduty-events-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/pagerduty/refs/heads/main/asyncapi/pagerduty-events-asyncapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "comodo.com"
  - 0 issuewild "digicert.com"
  - 0 iodef "mailto:ssl-tls-certificates-caa-iodef-report.r4785y6f@pdt-circular.pagerduty.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: pagerduty.com
  spf: true
hosts:
- cert_expires: Jan 22 23:59:59 2027 GMT
  host: developer.pagerduty.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 13:18:07 2026 GMT
  host: www.pagerduty.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 18 23:59:59 2027 GMT
  host: api.pagerduty.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Pagerduty Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PagerDuty, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: PagerDuty
provider_slug: pagerduty
slug: pagerduty-domain-security
source_filename: pagerduty-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.pagerduty.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.pagerduty.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 13:18:07 2026 GMT\n  hsts: false\n- host: api.pagerduty.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 18 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: pagerduty.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"comodo.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 iodef \"mailto:ssl-tls-certificates-caa-iodef-report.r4785y6f@pdt-circular.pagerduty.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pagerduty/refs/heads/main/security/pagerduty-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Alerting
- DevOps
- Incident Management
- On-Call Management
---
