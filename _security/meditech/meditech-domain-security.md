---
api_specs:
- filename: meditech-fhir-openapi.yml
  format: yaml
  label: Meditech Expanse FHIR API
  slug: meditech-expanse-fhir-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meditech/refs/heads/main/openapi/meditech-fhir-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "globalsign.com"
  - 0 issue "pki.goog"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: meditech.com
  spf: true
hosts:
- cert_expires: Sep 22 16:14:33 2026 GMT
  host: ehr.meditech.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 17:36:46 2026 GMT
  host: www.meditech.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Meditech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for meditech, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: meditech
provider_slug: meditech
slug: meditech-domain-security
source_filename: meditech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ehr.meditech.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 16:14:33 2026 GMT\n  hsts: false\n- host: www.meditech.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 17:36:46 2026 GMT\n  hsts: false\ndomains:\n- domain: meditech.com\n  dnssec: true\n  caa:\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/meditech/refs/heads/main/security/meditech-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags: []
---
