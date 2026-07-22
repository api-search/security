---
api_specs:
- filename: mon-ami-openapi.yml
  format: yaml
  label: Mon Ami REST API
  slug: mon-ami-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mon-ami/refs/heads/main/openapi/mon-ami-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 iodef "mailto:admin@monami.io"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: monami.io
  spf: true
hosts:
- cert_expires: Dec 22 23:59:59 2026 GMT
  host: www.monami.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mon Ami Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mon Ami, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Mon Ami
provider_slug: mon-ami
slug: mon-ami-domain-security
source_filename: mon-ami-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.monami.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: monami.io\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 iodef \"mailto:admin@monami.io\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mon-ami/refs/heads/main/security/mon-ami-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthcare
- Aging Services
- Disability Services
- Case Management
- Care Coordination
- HL7 FHIR
- HIPAA
---
