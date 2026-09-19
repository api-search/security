---
api_specs:
- filename: renaissance-lexile-api-openapi.yml
  format: yaml
  label: Lexile API
  slug: lexile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/renaissance/refs/heads/main/openapi/renaissance-lexile-api-openapi.yml
- filename: renaissance-classes-api-openapi.yml
  format: yaml
  label: Renaissance Classes API
  slug: renaissance-classes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/renaissance/refs/heads/main/openapi/renaissance-classes-api-openapi.yml
- filename: renaissance-events-api-openapi.yml
  format: yaml
  label: Renaissance Events API
  slug: renaissance-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/renaissance/refs/heads/main/openapi/renaissance-events-api-openapi.yml
- filename: renaissance-health-api-openapi.yml
  format: yaml
  label: Renaissance Health API
  slug: renaissance-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/renaissance/refs/heads/main/openapi/renaissance-health-api-openapi.yml
- filename: renaissance-pathway-api-openapi.yml
  format: yaml
  label: Renaissance Pathway API
  slug: renaissance-pathway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/renaissance/refs/heads/main/openapi/renaissance-pathway-api-openapi.yml
- filename: renaissance-predictions-api-openapi.yml
  format: yaml
  label: Renaissance Predictions API
  slug: renaissance-predictions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/renaissance/refs/heads/main/openapi/renaissance-predictions-api-openapi.yml
- filename: renaissance-reading-level-api-openapi.yml
  format: yaml
  label: Renaissance Reading Level API
  slug: renaissance-reading-level-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/renaissance/refs/heads/main/openapi/renaissance-reading-level-api-openapi.yml
- filename: renaissance-skills-api-openapi.yml
  format: yaml
  label: Renaissance Skills API
  slug: renaissance-skills-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/renaissance/refs/heads/main/openapi/renaissance-skills-api-openapi.yml
- filename: renaissance-utility-api-openapi.yml
  format: yaml
  label: Renaissance Utility API
  slug: renaissance-utility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/renaissance/refs/heads/main/openapi/renaissance-utility-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: renaissance.com
  spf: true
hosts:
- cert_expires: Oct 18 13:39:26 2026 GMT
  host: www.renaissance.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 18 23:59:59 2026 GMT
  host: proficiency.renaissance.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Mar  4 23:59:59 2027 GMT
  host: events.proficiency.renaissance.com
  hsts: null
  https: true
  tls_version: TLSv1.2
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Renaissance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Renaissance, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Renaissance
provider_slug: renaissance
slug: renaissance-domain-security
source_filename: renaissance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.renaissance.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 13:39:26 2026 GMT\n  hsts: false\n- host: proficiency.renaissance.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 18 23:59:59 2026 GMT\n  hsts: null\n- host: events.proficiency.renaissance.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar  4 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: renaissance.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/renaissance/refs/heads/main/security/renaissance-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Education
- EdTech
- K-12
- Assessment
- Learning Analytics
- Student Data
- OneRoster
- LTI
- Ed-Fi
- Rostering
- Interoperability
- Machine-Learning
---
