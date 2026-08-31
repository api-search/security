---
api_specs:
- filename: 2sAY548Kou
  format: yaml
  label: TalentLMS API
  slug: talentlms-api
  spec_type: Postman
  url: https://documenter.getpostman.com/view/31867199/2sAY548Kou
- filename: talentlms-batch-actions-api-openapi.yml
  format: yaml
  label: TalentLMS Batch Actions API
  slug: talentlms-batch-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talentlms/refs/heads/main/openapi/talentlms-batch-actions-api-openapi.yml
- filename: talentlms-branch-api-openapi.yml
  format: yaml
  label: TalentLMS Branch API
  slug: talentlms-branch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talentlms/refs/heads/main/openapi/talentlms-branch-api-openapi.yml
- filename: talentlms-category-api-openapi.yml
  format: yaml
  label: TalentLMS Category API
  slug: talentlms-category-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talentlms/refs/heads/main/openapi/talentlms-category-api-openapi.yml
- filename: talentlms-course-api-openapi.yml
  format: yaml
  label: TalentLMS Course API
  slug: talentlms-course-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talentlms/refs/heads/main/openapi/talentlms-course-api-openapi.yml
- filename: talentlms-group-api-openapi.yml
  format: yaml
  label: TalentLMS Group API
  slug: talentlms-group-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talentlms/refs/heads/main/openapi/talentlms-group-api-openapi.yml
- filename: talentlms-learning-paths-api-openapi.yml
  format: yaml
  label: TalentLMS Learning Paths API
  slug: talentlms-learning-paths-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talentlms/refs/heads/main/openapi/talentlms-learning-paths-api-openapi.yml
- filename: talentlms-portal-api-openapi.yml
  format: yaml
  label: TalentLMS Portal API
  slug: talentlms-portal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talentlms/refs/heads/main/openapi/talentlms-portal-api-openapi.yml
- filename: talentlms-task-api-openapi.yml
  format: yaml
  label: TalentLMS Task API
  slug: talentlms-task-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talentlms/refs/heads/main/openapi/talentlms-task-api-openapi.yml
- filename: talentlms-timeline-api-openapi.yml
  format: yaml
  label: TalentLMS Timeline API
  slug: talentlms-timeline-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talentlms/refs/heads/main/openapi/talentlms-timeline-api-openapi.yml
- filename: talentlms-unit-api-openapi.yml
  format: yaml
  label: TalentLMS Unit API
  slug: talentlms-unit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talentlms/refs/heads/main/openapi/talentlms-unit-api-openapi.yml
- filename: talentlms-user-api-openapi.yml
  format: yaml
  label: TalentLMS User API
  slug: talentlms-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talentlms/refs/heads/main/openapi/talentlms-user-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: talentlms.io
  spf: false
- caa:
  - 0 issuewild "amazon.com"
  - 0 issuewild "comodo.com"
  - 0 issuewild "digicert.com"
  - 0 issuewild "entrust.net"
  - 0 issuewild "globalsign.com"
  - 0 issuewild "godaddy.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: talentlms.com
  spf: true
hosts:
- cert_expires: Oct  5 10:24:48 2026 GMT
  host: developers.talentlms.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 11 23:59:59 2026 GMT
  host: your-domain.talentlms.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Talentlms Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TalentLMS, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: TalentLMS
provider_slug: talentlms
slug: talentlms-domain-security
source_filename: talentlms-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.talentlms.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 10:24:48 2026 GMT\n  hsts: false\n- host: your-domain.talentlms.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: talentlms.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: talentlms.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"comodo.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"entrust.net\"\n  - 0 issuewild \"globalsign.com\"\n  - 0 issuewild \"godaddy.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/talentlms/refs/heads/main/security/talentlms-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Learning Management System
- LMS
- eLearning
- Training
- Courses
- User
- Enrollments
- Education
- HR Tech
- Cloud
---
