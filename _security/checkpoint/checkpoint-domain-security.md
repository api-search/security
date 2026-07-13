---
api_specs:
- filename: checkpoint-management-api-openapi.yml
  format: yaml
  label: Check Point Management API
  slug: management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkpoint/refs/heads/main/openapi/checkpoint-management-api-openapi.yml
- filename: checkpoint-gaia-api-openapi.yml
  format: yaml
  label: Check Point Gaia API
  slug: gaia-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkpoint/refs/heads/main/openapi/checkpoint-gaia-api-openapi.yml
- filename: checkpoint-cloudguard-api-openapi.yml
  format: yaml
  label: Check Point CloudGuard API
  slug: cloudguard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkpoint/refs/heads/main/openapi/checkpoint-cloudguard-api-openapi.yml
- filename: checkpoint-identity-awareness-api-openapi.yml
  format: yaml
  label: Check Point Identity Awareness API
  slug: identity-awareness-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkpoint/refs/heads/main/openapi/checkpoint-identity-awareness-api-openapi.yml
- filename: checkpoint-harmony-email-api-openapi.yml
  format: yaml
  label: Check Point Harmony Email API
  slug: harmony-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkpoint/refs/heads/main/openapi/checkpoint-harmony-email-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "globalsign.com"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "amazon.com"
  - 0 iodef "mailto:hostmaster@checkpoint.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: checkpoint.com
  spf: true
hosts:
- cert_expires: Jan  2 06:44:08 2027 GMT
  host: www.checkpoint.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  2 23:59:59 2027 GMT
  host: sc1.checkpoint.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 09:25:52 2026 GMT
  host: docs.cgn.portal.checkpoint.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Checkpoint Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Check Point, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Check Point
provider_slug: checkpoint
slug: checkpoint-domain-security
source_filename: checkpoint-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.checkpoint.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 06:44:08 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: sc1.checkpoint.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  2 23:59:59 2027 GMT\n  hsts: false\n- host: docs.cgn.portal.checkpoint.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 09:25:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: checkpoint.com\n  dnssec: true\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"globalsign.com\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"amazon.com\"\n  - 0 iodef \"mailto:hostmaster@checkpoint.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/checkpoint/refs/heads/main/security/checkpoint-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Cloud Security
- Cybersecurity
- Endpoint Security
- Firewall
- Identity Awareness
- Mobile Security
- Network Security
- Security
- Threat Prevention
- WAF
---
