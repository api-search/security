---
api_specs:
- filename: vivalink-openapi.yml
  format: yaml
  label: VivaLNK Subjects API
  slug: vivalink-subjects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vivalink/refs/heads/main/openapi/vivalink-openapi.yml
- filename: vivalink-openapi.yml
  format: yaml
  label: VivaLNK Devices API
  slug: vivalink-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vivalink/refs/heads/main/openapi/vivalink-openapi.yml
- filename: vivalink-openapi.yml
  format: yaml
  label: VivaLNK Vital Signs Data API
  slug: vivalink-vital-signs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vivalink/refs/heads/main/openapi/vivalink-openapi.yml
- filename: vivalink-openapi.yml
  format: yaml
  label: VivaLNK Webhooks API
  slug: vivalink-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vivalink/refs/heads/main/openapi/vivalink-openapi.yml
- filename: vivalink-openapi.yml
  format: yaml
  label: VivaLNK FHIR API
  slug: vivalink-fhir-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vivalink/refs/heads/main/openapi/vivalink-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: vivalink.com
  spf: true
hosts:
- cert_expires: Sep 20 08:05:35 2026 GMT
  host: www.vivalink.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 02:54:23 2026 GMT
  host: api.vivalink.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vivalink Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for VivaLNK, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: VivaLNK
provider_slug: vivalink
slug: vivalink-domain-security
source_filename: vivalink-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vivalink.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 08:05:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.vivalink.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 02:54:23 2026 GMT\n  hsts: null\ndomains:\n- domain: vivalink.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vivalink/refs/heads/main/security/vivalink-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Connected Health
- Remote Patient Monitoring
- RPM
- Wearables
- Biosensors
- Biometrics
- ECG
- Vital Signs
- Digital Health
- IoT
- Clinical Trials
---
