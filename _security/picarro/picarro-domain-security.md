---
api_specs:
- filename: picarro-sam-foup-asyncapi.yml
  format: yaml
  label: Picarro Edge — SAM FOUP gRPC API
  slug: picarro-edge-sam-foup-grpc-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/picarro/refs/heads/main/asyncapi/picarro-sam-foup-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: picarro.com
  spf: true
hosts:
- cert_expires: Oct 18 03:19:36 2026 GMT
  host: www.picarro.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  2 23:59:59 2027 GMT
  host: pcubed.picarro.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan  2 23:59:59 2027 GMT
  host: identity-prod.picarro.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Picarro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Picarro, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Picarro
provider_slug: picarro
slug: picarro-domain-security
source_filename: picarro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.picarro.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 03:19:36 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: pcubed.picarro.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  2 23:59:59 2027 GMT\n  hsts: null\n- host: identity-prod.picarro.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  2 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: picarro.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/picarro/refs/heads/main/security/picarro-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Gas Detection
- Environmental Monitoring
- Emissions
- Methane
- Greenhouse Gas
- Scientific Instruments
- Semiconductors
- Industrial IoT
- Sensors
- Analytics
- gRPC
---
