---
api_specs:
- filename: tennet-openapi-generated.yml
  format: yaml
  label: TenneT API
  slug: tennet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tennet/refs/heads/main/openapi/_ae-authored/tennet-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:certificatemanagement@tennet.eu"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tennet.eu
  spf: true
hosts:
- cert_expires: Jan 22 23:59:59 2027 GMT
  host: www.tennet.eu
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Tennet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TenneT, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: TenneT
provider_slug: tennet
slug: tennet-domain-security
source_filename: tennet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tennet.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: tennet.eu\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:certificatemanagement@tennet.eu\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tennet/refs/heads/main/security/tennet-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Energy
- Transmission
- Grid Operator
- Europe
- Sustainability
- Company
---
