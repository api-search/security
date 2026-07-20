---
api_specs:
- filename: devoted-patient-access-openapi.json
  format: json
  label: Patient Access API
  slug: patient-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/devoted/refs/heads/main/openapi/devoted-patient-access-openapi.json
description: ''
domains:
- caa:
  - 128 issue "letsencrypt.org;validationmethods=dns-01;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/2119334475"
  - 128 issue "letsencrypt.org;validationmethods=dns-01;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/88814841"
  - 128 issue "sectigo.com"
  - 128 issue "amazonaws.com"
  - 128 issue "digicert.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: devoted.com
  spf: true
hosts:
- cert_expires: Oct  1 23:59:59 2026 GMT
  host: devoted.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 18 15:16:55 2026 GMT
  host: api.prod.devoted.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Devoted Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Devoted Health, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Devoted Health
provider_slug: devoted
slug: devoted-domain-security
source_filename: devoted-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: devoted.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.prod.devoted.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 15:16:55 2026 GMT\n  hsts: null\ndomains:\n- domain: devoted.com\n  dnssec: true\n  caa:\n  - 128 issue \"letsencrypt.org;validationmethods=dns-01;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/2119334475\"\n  - 128 issue \"letsencrypt.org;validationmethods=dns-01;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/88814841\"\n  - 128 issue \"sectigo.com\"\n  - 128 issue \"amazonaws.com\"\n  - 128 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/devoted/refs/heads/main/security/devoted-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Healthcare
- Medicare Advantage
- Health Insurance
- FHIR
- Interoperability
- CMS Patient Access
- Payer
---
