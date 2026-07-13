---
api_specs:
- filename: adobe-analytics-api-openapi.yml
  format: yaml
  label: Adobe Analytics 2.0 API
  slug: analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/openapi/adobe-analytics-api-openapi.yml
- filename: adobe-experience-platform-api-openapi.yml
  format: yaml
  label: Adobe Experience Platform API
  slug: experience-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/openapi/adobe-experience-platform-api-openapi.yml
- filename: adobe-target-api-openapi.yml
  format: yaml
  label: Adobe Target API
  slug: target-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/openapi/adobe-target-api-openapi.yml
- filename: adobe-journey-optimizer-api-openapi.yml
  format: yaml
  label: Adobe Journey Optimizer API
  slug: journey-optimizer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/openapi/adobe-journey-optimizer-api-openapi.yml
- filename: adobe-campaign-api-openapi.yml
  format: yaml
  label: Adobe Campaign API
  slug: campaign-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/openapi/adobe-campaign-api-openapi.yml
- filename: adobe-io-events-asyncapi.yml
  format: yaml
  label: Adobe I/O Events
  slug: io-events
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/asyncapi/adobe-io-events-asyncapi.yml
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
- cert_expires: Nov 26 23:59:59 2026 GMT
  host: analytics.adobe.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 26 23:59:59 2026 GMT
  host: platform.adobe.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Adobe Experience Cloud Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Adobe Experience Cloud, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Adobe Experience Cloud
provider_slug: adobe-experience-cloud
slug: adobe-experience-cloud-domain-security
source_filename: adobe-experience-cloud-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.adobe.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  7 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: analytics.adobe.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 23:59:59 2026 GMT\n  hsts: null\n- host: platform.adobe.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: adobe.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: adobe.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/security/adobe-experience-cloud-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Analytics
- Customer Experience
- Digital Marketing
- Personalization
- Campaign Management
- Journey Orchestration
---
