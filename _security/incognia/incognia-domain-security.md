---
api_specs:
- filename: incognia-openapi-original.yml
  format: yaml
  label: Incognia API
  slug: incognia-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/incognia/refs/heads/main/openapi/incognia-openapi-original.yml
description: ''
domains:
- caa:
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "awstrust.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: incognia.com
  spf: true
hosts:
- cert_expires: Sep 20 03:32:43 2026 GMT
  host: www.incognia.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 12 23:59:59 2027 GMT
  host: developer.incognia.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 23 23:59:59 2026 GMT
  host: api.incognia.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Incognia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Incognia, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Incognia
provider_slug: incognia
slug: incognia-domain-security
source_filename: incognia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.incognia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 03:32:43 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.incognia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.incognia.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 23 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: incognia.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/incognia/refs/heads/main/security/incognia-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Cybersecurity
- Fraud Prevention
- Device Fingerprinting
- Location Identity
- Identity Verification
- Risk Assessment
- Authentication
- Fintech
- Anti-Fraud
---
