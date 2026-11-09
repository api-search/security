---
api_specs:
- filename: dmarc-examiner-com-alerts-api-openapi.yml
  format: yaml
  label: DMARC Examiner Alerts API
  slug: dmarc-examiner-com-alerts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dmarc-examiner-com/openapi/dmarc-examiner-com-alerts-api-openapi.yml
- filename: dmarc-examiner-com-domains-api-openapi.yml
  format: yaml
  label: DMARC Examiner Domains API
  slug: dmarc-examiner-com-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dmarc-examiner-com/openapi/dmarc-examiner-com-domains-api-openapi.yml
- filename: dmarc-examiner-com-forensic-reports-api-openapi.yml
  format: yaml
  label: DMARC Examiner Forensic Reports API
  slug: dmarc-examiner-com-forensic-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dmarc-examiner-com/openapi/dmarc-examiner-com-forensic-reports-api-openapi.yml
- filename: dmarc-examiner-com-reports-api-openapi.yml
  format: yaml
  label: DMARC Examiner Reports API
  slug: dmarc-examiner-com-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dmarc-examiner-com/openapi/dmarc-examiner-com-reports-api-openapi.yml
- filename: dmarc-examiner-com-tools-api-openapi.yml
  format: yaml
  label: DMARC Examiner Tools API
  slug: dmarc-examiner-com-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dmarc-examiner-com/openapi/dmarc-examiner-com-tools-api-openapi.yml
- filename: dmarc-examiner-com-webhooks-api-openapi.yml
  format: yaml
  label: DMARC Examiner Webhooks API
  slug: dmarc-examiner-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dmarc-examiner-com/openapi/dmarc-examiner-com-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: dmarc-examiner.com
  spf: true
hosts:
- cert_expires: Dec 19 02:02:05 2026 GMT
  host: dmarc-examiner.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dmarc Examiner Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DMARC Examiner, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: DMARC Examiner
provider_slug: dmarc-examiner-com
slug: dmarc-examiner-com-domain-security
source_filename: dmarc-examiner-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dmarc-examiner.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 02:02:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: dmarc-examiner.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/dmarc-examiner-com/security/dmarc-examiner-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Email Security
- DMARC
- SPF
- DKIM
- Anti-Phishing
- Monitoring
---
