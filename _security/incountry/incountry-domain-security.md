---
api_specs:
- filename: RestAPI_Demo_oAuth.postman_collection-e8b012cac5488563ba466e6ea44c309c.json
  format: json
  label: InCountry REST API
  slug: incountry-rest-api
  spec_type: Postman
  url: https://docs.incountry.com/assets/files/RestAPI_Demo_oAuth.postman_collection-e8b012cac5488563ba466e6ea44c309c.json
description: ''
domains:
- caa:
  - 0 iodef "mailto:opsmgt@incountry.com"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: incountry.com
  spf: true
hosts:
- cert_expires: Aug 23 07:23:32 2026 GMT
  host: incountry.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Incountry Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for InCountry, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: InCountry
provider_slug: incountry
slug: incountry-domain-security
source_filename: incountry-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: incountry.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 07:23:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: incountry.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:opsmgt@incountry.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/incountry/refs/heads/main/security/incountry-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Data Residency
- Data Localization
- Compliance
- Privacy
- Data Security
- Encryption
- PII
- GDPR
- Data Sovereignty
- MCP
---
