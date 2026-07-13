---
api_specs:
- filename: adobe-firefly-api-openapi-original.yml
  format: yaml
  label: Adobe Firefly API
  slug: firefly-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-cloud/refs/heads/main/openapi/adobe-firefly-api-openapi-original.yml
- filename: adobe-cc-libraries-api-openapi-original.yml
  format: yaml
  label: Creative Cloud Libraries API
  slug: cc-libraries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-cloud/refs/heads/main/openapi/adobe-cc-libraries-api-openapi-original.yml
- filename: adobe-stock-api-openapi-original.yml
  format: yaml
  label: Adobe Stock API
  slug: stock-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-cloud/refs/heads/main/openapi/adobe-stock-api-openapi-original.yml
- filename: adobe-pdf-services-api-openapi-original.yml
  format: yaml
  label: Adobe PDF Services API
  slug: pdf-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-cloud/refs/heads/main/openapi/adobe-pdf-services-api-openapi-original.yml
- filename: adobe-io-events-asyncapi-original.yml
  format: yaml
  label: Adobe I/O Events
  slug: io-events
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-cloud/refs/heads/main/asyncapi/adobe-io-events-asyncapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: adobe.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: adobe.io
  spf: true
hosts:
- cert_expires: Dec  7 23:59:59 2026 GMT
  host: developer.adobe.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan  4 23:59:59 2027 GMT
  host: www.adobe.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 28 23:59:59 2026 GMT
  host: firefly-api.adobe.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Adobe Creative Cloud Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Adobe Creative Cloud, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Adobe Creative Cloud
provider_slug: adobe-creative-cloud
slug: adobe-creative-cloud-domain-security
source_filename: adobe-creative-cloud-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.adobe.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  7 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: www.adobe.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 23:59:59 2027 GMT\n  hsts: null\n- host: firefly-api.adobe.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: adobe.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: adobe.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-cloud/refs/heads/main/security/adobe-creative-cloud-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- AI/ML
- Cloud
- Creative
- Design
- Documents
- Photography
- SaaS
- Video
---
