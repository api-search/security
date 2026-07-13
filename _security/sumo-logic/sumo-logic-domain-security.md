---
api_specs:
- filename: sumo-logic-openapi.yml
  format: yaml
  label: Sumo Logic API
  slug: sumo-logic
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sumo-logic/refs/heads/main/openapi/sumo-logic-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "geotrust.com"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: sumologic.com
  spf: true
hosts:
- host: developer.sumologic.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has expired (_ssl.c:1082)'
- cert_expires: Sep 16 16:38:31 2026 GMT
  host: www.sumologic.com
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  7 23:59:59 2027 GMT
  host: help.sumologic.com
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Sumo Logic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sumo Logic, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Sumo Logic
provider_slug: sumo-logic
slug: sumo-logic-domain-security
source_filename: sumo-logic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.sumologic.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has\n    expired (_ssl.c:1082)'\n  hsts: null\n- host: www.sumologic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 16:38:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31622400\n- host: help.sumologic.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar  7 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31622400\ndomains:\n- domain: sumologic.com\n  dnssec: true\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"geotrust.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sumo-logic/refs/heads/main/security/sumo-logic-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Logging
- Observability
- Security
- Monitoring
- Analytics
- DevOps
- SIEM
---
