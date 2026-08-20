---
api_specs:
- filename: adobe-captivate-learning-manager-webhooks-asyncapi.yml
  format: yaml
  label: Adobe Learning Manager Webhooks API
  slug: adobe-learning-manager-webhooks-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-captivate/refs/heads/main/asyncapi/adobe-captivate-learning-manager-webhooks-asyncapi.yml
- filename: adobe-captivate-account-api-openapi.yml
  format: yaml
  label: Adobe Captivate Account API
  slug: adobe-captivate-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-captivate/refs/heads/main/openapi/adobe-captivate-account-api-openapi.yml
- filename: adobe-captivate-badges-api-openapi.yml
  format: yaml
  label: Adobe Captivate Badges API
  slug: adobe-captivate-badges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-captivate/refs/heads/main/openapi/adobe-captivate-badges-api-openapi.yml
- filename: adobe-captivate-catalogs-api-openapi.yml
  format: yaml
  label: Adobe Captivate Catalogs API
  slug: adobe-captivate-catalogs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-captivate/refs/heads/main/openapi/adobe-captivate-catalogs-api-openapi.yml
- filename: adobe-captivate-certifications-api-openapi.yml
  format: yaml
  label: Adobe Captivate Certifications API
  slug: adobe-captivate-certifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-captivate/refs/heads/main/openapi/adobe-captivate-certifications-api-openapi.yml
- filename: adobe-captivate-enrollments-api-openapi.yml
  format: yaml
  label: Adobe Captivate Enrollments API
  slug: adobe-captivate-enrollments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-captivate/refs/heads/main/openapi/adobe-captivate-enrollments-api-openapi.yml
- filename: adobe-captivate-gamification-api-openapi.yml
  format: yaml
  label: Adobe Captivate Gamification API
  slug: adobe-captivate-gamification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-captivate/refs/heads/main/openapi/adobe-captivate-gamification-api-openapi.yml
- filename: adobe-captivate-jobs-api-openapi.yml
  format: yaml
  label: Adobe Captivate Jobs API
  slug: adobe-captivate-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-captivate/refs/heads/main/openapi/adobe-captivate-jobs-api-openapi.yml
- filename: adobe-captivate-learning-objects-api-openapi.yml
  format: yaml
  label: Adobe Captivate Learning Objects API
  slug: adobe-captivate-learning-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-captivate/refs/heads/main/openapi/adobe-captivate-learning-objects-api-openapi.yml
- filename: adobe-captivate-notifications-api-openapi.yml
  format: yaml
  label: Adobe Captivate Notifications API
  slug: adobe-captivate-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-captivate/refs/heads/main/openapi/adobe-captivate-notifications-api-openapi.yml
- filename: adobe-captivate-skills-api-openapi.yml
  format: yaml
  label: Adobe Captivate Skills API
  slug: adobe-captivate-skills-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-captivate/refs/heads/main/openapi/adobe-captivate-skills-api-openapi.yml
- filename: adobe-captivate-user-groups-api-openapi.yml
  format: yaml
  label: Adobe Captivate User Groups API
  slug: adobe-captivate-user-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-captivate/refs/heads/main/openapi/adobe-captivate-user-groups-api-openapi.yml
- filename: adobe-captivate-users-api-openapi.yml
  format: yaml
  label: Adobe Captivate Users API
  slug: adobe-captivate-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-captivate/refs/heads/main/openapi/adobe-captivate-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: adobe.com
  spf: true
hosts:
- cert_expires: Sep 30 23:59:59 2026 GMT
  host: experienceleague.adobe.com
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  4 23:59:59 2027 GMT
  host: business.adobe.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  4 23:59:59 2027 GMT
  host: www.adobe.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Adobe Captivate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Adobe Captivate, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Adobe Captivate
provider_slug: adobe-captivate
slug: adobe-captivate-domain-security
source_filename: adobe-captivate-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: experienceleague.adobe.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\n- host: business.adobe.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 23:59:59 2027 GMT\n  hsts: null\n- host: www.adobe.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: adobe.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adobe-captivate/refs/heads/main/security/adobe-captivate-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Authoring
- Education
- E-Learning
- LMS
- SCORM
- Training
- xAPI
---
