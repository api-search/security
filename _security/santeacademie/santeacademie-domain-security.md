---
api_specs:
- filename: santeacademie-article-api-openapi.yml
  format: yaml
  label: Santé Académie Article API
  slug: santeacademie-article-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/santeacademie/refs/heads/main/openapi/santeacademie-article-api-openapi.yml
- filename: santeacademie-customcatalog-api-openapi.yml
  format: yaml
  label: Santé Académie Custom Catalog API
  slug: santeacademie-customcatalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/santeacademie/refs/heads/main/openapi/santeacademie-customcatalog-api-openapi.yml
- filename: santeacademie-faq-api-openapi.yml
  format: yaml
  label: Santé Académie Faq API
  slug: santeacademie-faq-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/santeacademie/refs/heads/main/openapi/santeacademie-faq-api-openapi.yml
- filename: santeacademie-health-facility-api-openapi.yml
  format: yaml
  label: Santé Académie Health Facility API
  slug: santeacademie-health-facility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/santeacademie/refs/heads/main/openapi/santeacademie-health-facility-api-openapi.yml
- filename: santeacademie-job-api-openapi.yml
  format: yaml
  label: Santé Académie Job API
  slug: santeacademie-job-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/santeacademie/refs/heads/main/openapi/santeacademie-job-api-openapi.yml
- filename: santeacademie-jobspace-api-openapi.yml
  format: yaml
  label: Santé Académie Job Space API
  slug: santeacademie-jobspace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/santeacademie/refs/heads/main/openapi/santeacademie-jobspace-api-openapi.yml
- filename: santeacademie-mediacategory-api-openapi.yml
  format: yaml
  label: Santé Académie Media Category API
  slug: santeacademie-mediacategory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/santeacademie/refs/heads/main/openapi/santeacademie-mediacategory-api-openapi.yml
- filename: santeacademie-pharmacy-api-openapi.yml
  format: yaml
  label: Santé Académie Pharmacy API
  slug: santeacademie-pharmacy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/santeacademie/refs/heads/main/openapi/santeacademie-pharmacy-api-openapi.yml
- filename: santeacademie-resource-api-openapi.yml
  format: yaml
  label: Santé Académie Resource API
  slug: santeacademie-resource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/santeacademie/refs/heads/main/openapi/santeacademie-resource-api-openapi.yml
- filename: santeacademie-sitemap-api-openapi.yml
  format: yaml
  label: Santé Académie Sitemap API
  slug: santeacademie-sitemap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/santeacademie/refs/heads/main/openapi/santeacademie-sitemap-api-openapi.yml
- filename: santeacademie-testimonial-api-openapi.yml
  format: yaml
  label: Santé Académie Testimonial API
  slug: santeacademie-testimonial-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/santeacademie/refs/heads/main/openapi/santeacademie-testimonial-api-openapi.yml
- filename: santeacademie-topic-api-openapi.yml
  format: yaml
  label: Santé Académie Topic API
  slug: santeacademie-topic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/santeacademie/refs/heads/main/openapi/santeacademie-topic-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: santeacademie.com
  spf: true
hosts:
- cert_expires: Feb  7 23:59:59 2027 GMT
  host: www.santeacademie.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 11 04:26:04 2026 GMT
  host: frontstage.santeacademie.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Santeacademie Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Santé Académie, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Santé Académie
provider_slug: santeacademie
slug: santeacademie-domain-security
source_filename: santeacademie-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.santeacademie.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  7 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: frontstage.santeacademie.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 04:26:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: santeacademie.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/santeacademie/refs/heads/main/security/santeacademie-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- EdTech
- Healthcare Training
- Continuing Education
- DPC
- E-Learning
- France
- Healthcare Professionals
- Course Catalog
- LMS
---
