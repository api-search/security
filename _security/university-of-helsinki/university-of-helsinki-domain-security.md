---
api_specs:
- filename: university-of-helsinki-hy-organisation-api-openapi.yml
  format: yaml
  label: HY Organisation API
  slug: hy-organisation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-helsinki/refs/heads/main/openapi/university-of-helsinki-hy-organisation-api-openapi.yml
- filename: university-of-helsinki-contact-search-api-openapi.yml
  format: yaml
  label: Contact Search API
  slug: contact-search
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-helsinki/refs/heads/main/openapi/university-of-helsinki-contact-search-api-openapi.yml
- filename: university-of-helsinki-course-pages-cms-openapi.yml
  format: yaml
  label: Course pages CMS
  slug: course-pages-cms
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-helsinki/refs/heads/main/openapi/university-of-helsinki-course-pages-cms-openapi.yml
- filename: university-of-helsinki-helsinki-fi-content-openapi.yml
  format: yaml
  label: Helsinki.fi content
  slug: helsinki-fi-content
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-helsinki/refs/heads/main/openapi/university-of-helsinki-helsinki-fi-content-openapi.yml
- filename: university-of-helsinki-hy-building-api-openapi.yml
  format: yaml
  label: HY Building API
  slug: hy-building
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-helsinki/refs/heads/main/openapi/university-of-helsinki-hy-building-api-openapi.yml
- filename: university-of-helsinki-serviceapi-openapi.yml
  format: yaml
  label: ServiceAPI
  slug: serviceapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-helsinki/refs/heads/main/openapi/university-of-helsinki-serviceapi-openapi.yml
- filename: university-of-helsinki-employeeinformationapi-openapi.yml
  format: yaml
  label: EmployeeInformationAPI
  slug: employeeinformation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-helsinki/refs/heads/main/openapi/university-of-helsinki-employeeinformationapi-openapi.yml
- filename: university-of-helsinki-persongroup-openapi.yml
  format: yaml
  label: PersonGroup
  slug: persongroup
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-helsinki/refs/heads/main/openapi/university-of-helsinki-persongroup-openapi.yml
- filename: university-of-helsinki-general-efecte-api-openapi.yml
  format: yaml
  label: General Efecte API
  slug: general-efecte
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-helsinki/refs/heads/main/openapi/university-of-helsinki-general-efecte-api-openapi.yml
- filename: university-of-helsinki-network-registry-api-openapi.yml
  format: yaml
  label: Network registry API
  slug: network-registry
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-helsinki/refs/heads/main/openapi/university-of-helsinki-network-registry-api-openapi.yml
- filename: university-of-helsinki-sovellussalkku-api-openapi.yml
  format: yaml
  label: Sovellussalkku API
  slug: sovellussalkku
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-helsinki/refs/heads/main/openapi/university-of-helsinki-sovellussalkku-api-openapi.yml
- filename: university-of-helsinki-dawa-sync-api-openapi.yml
  format: yaml
  label: Dawa Sync API
  slug: dawa-sync
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-helsinki/refs/heads/main/openapi/university-of-helsinki-dawa-sync-api-openapi.yml
- filename: university-of-helsinki-finbif-laji-openapi.yml
  format: yaml
  label: FinBIF Laji API (Finnish Biodiversity Information Facility)
  slug: finbif-laji
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-helsinki/refs/heads/main/openapi/university-of-helsinki-finbif-laji-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: helsinki.fi
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: funidata.fi
  spf: true
hosts:
- cert_expires: Sep 29 03:26:17 2026 GMT
  host: www.helsinki.fi
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 19:19:44 2026 GMT
  host: helda.helsinki.fi
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 05:43:52 2026 GMT
  host: www.funidata.fi
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: University Of Helsinki Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of Helsinki, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: University of Helsinki
provider_slug: university-of-helsinki
slug: university-of-helsinki-domain-security
source_filename: university-of-helsinki-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.helsinki.fi\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 03:26:17 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: helda.helsinki.fi\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 19:19:44 2026 GMT\n  hsts: false\n- host: www.funidata.fi\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 05:43:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: helsinki.fi\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: funidata.fi\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-helsinki/refs/heads/main/security/university-of-helsinki-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Finland
- Nordic
- Research
- Open Data
- Research Data
- Institutional Repository
- OAI-PMH
- Identity Federation
- API Gateway
- Course Catalog
- Library
- Biodiversity
---
