---
api_specs:
- filename: lingopal-jobs-api-openapi.yml
  format: yaml
  label: Lingopal Jobs API
  slug: lingopal-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lingopal/openapi/lingopal-jobs-api-openapi.yml
- filename: lingopal-languages-api-openapi.yml
  format: yaml
  label: Lingopal Languages API
  slug: lingopal-languages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lingopal/openapi/lingopal-languages-api-openapi.yml
- filename: lingopal-job-outputs-api-openapi.yml
  format: yaml
  label: Lingopal Job Outputs API
  slug: lingopal-job-outputs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lingopal/openapi/lingopal-job-outputs-api-openapi.yml
- filename: lingopal-job-registration-api-openapi.yml
  format: yaml
  label: Lingopal Job Registration API
  slug: lingopal-job-registration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lingopal/openapi/lingopal-job-registration-api-openapi.yml
- filename: lingopal-job-workflows-api-openapi.yml
  format: yaml
  label: Lingopal Job Workflows API
  slug: lingopal-job-workflows-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lingopal/openapi/lingopal-job-workflows-api-openapi.yml
- filename: lingopal-storage-api-openapi.yml
  format: yaml
  label: Lingopal Storage API
  slug: lingopal-storage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lingopal/openapi/lingopal-storage-api-openapi.yml
- filename: lingopal-text-translation-api-openapi.yml
  format: yaml
  label: Lingopal Text Translation API
  slug: lingopal-text-translation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lingopal/openapi/lingopal-text-translation-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lingopal.ai
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: lingopal-dev.com
  spf: false
hosts:
- cert_expires: Nov 18 23:59:59 2026 GMT
  host: lingopal.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 14 23:59:59 2026 GMT
  host: vod-api.lingopal-dev.com
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Lingopal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lingopal, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Lingopal
provider_slug: lingopal
slug: lingopal-domain-security
source_filename: lingopal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lingopal.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 18 23:59:59 2026 GMT\n  hsts: false\n- host: vod-api.lingopal-dev.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 14 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: lingopal.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: lingopal-dev.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/lingopal/security/lingopal-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Frontier Tech
- Artificial Intelligence
- Translation
- Localization
- Speech
- Media
- Broadcasting
- Video
- Subtitles
- Voice Cloning
---
