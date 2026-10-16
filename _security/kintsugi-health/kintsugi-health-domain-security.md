---
api_specs:
- filename: kintsugi-health-openapi-generated.yml
  format: yaml
  label: Kintsugi Health API
  slug: kintsugi-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kintsugi-health/refs/heads/main/openapi/_ae-authored/kintsugi-health-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: kintsugihealth.com
  spf: true
hosts:
- cert_expires: Nov 27 03:47:10 2026 GMT
  host: www.kintsugihealth.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Kintsugi Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kintsugi Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Kintsugi Health
provider_slug: kintsugi-health
slug: kintsugi-health-domain-security
source_filename: kintsugi-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kintsugihealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 03:47:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: kintsugihealth.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kintsugi-health/refs/heads/main/security/kintsugi-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- HealthTech
- AI
- VoiceAnalytics
- MentalHealth
- DigitalHealth
---
