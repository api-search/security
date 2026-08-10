---
api_specs:
- filename: ethernovia-audit-user-trail-api-openapi.yml
  format: yaml
  label: Ethernovia Audit User Trail API
  slug: ethernovia-audit-user-trail-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ethernovia/refs/heads/main/openapi/ethernovia-audit-user-trail-api-openapi.yml
- filename: ethernovia-ec-document-api-openapi.yml
  format: yaml
  label: Ethernovia Ec Document API
  slug: ethernovia-ec-document-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ethernovia/refs/heads/main/openapi/ethernovia-ec-document-api-openapi.yml
- filename: ethernovia-ec-document-type-api-openapi.yml
  format: yaml
  label: Ethernovia Ec Document Type API
  slug: ethernovia-ec-document-type-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ethernovia/refs/heads/main/openapi/ethernovia-ec-document-type-api-openapi.yml
- filename: ethernovia-ec-excluded-domain-api-openapi.yml
  format: yaml
  label: Ethernovia Ec Excluded Domain API
  slug: ethernovia-ec-excluded-domain-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ethernovia/refs/heads/main/openapi/ethernovia-ec-excluded-domain-api-openapi.yml
- filename: ethernovia-ec-group-api-openapi.yml
  format: yaml
  label: Ethernovia Ec Group API
  slug: ethernovia-ec-group-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ethernovia/refs/heads/main/openapi/ethernovia-ec-group-api-openapi.yml
- filename: ethernovia-ec-product-api-openapi.yml
  format: yaml
  label: Ethernovia Ec Product API
  slug: ethernovia-ec-product-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ethernovia/refs/heads/main/openapi/ethernovia-ec-product-api-openapi.yml
- filename: ethernovia-ec-product-category-api-openapi.yml
  format: yaml
  label: Ethernovia Ec Product Category API
  slug: ethernovia-ec-product-category-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ethernovia/refs/heads/main/openapi/ethernovia-ec-product-category-api-openapi.yml
- filename: ethernovia-ec-product-family-api-openapi.yml
  format: yaml
  label: Ethernovia Ec Product Family API
  slug: ethernovia-ec-product-family-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ethernovia/refs/heads/main/openapi/ethernovia-ec-product-family-api-openapi.yml
- filename: ethernovia-ec-send-alert-email-api-openapi.yml
  format: yaml
  label: Ethernovia Ec Send Alert Email API
  slug: ethernovia-ec-send-alert-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ethernovia/refs/heads/main/openapi/ethernovia-ec-send-alert-email-api-openapi.yml
- filename: ethernovia-ec-software-package-api-openapi.yml
  format: yaml
  label: Ethernovia Ec Software Package API
  slug: ethernovia-ec-software-package-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ethernovia/refs/heads/main/openapi/ethernovia-ec-software-package-api-openapi.yml
- filename: ethernovia-ec-status-api-openapi.yml
  format: yaml
  label: Ethernovia Ec Status API
  slug: ethernovia-ec-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ethernovia/refs/heads/main/openapi/ethernovia-ec-status-api-openapi.yml
- filename: ethernovia-my-download-api-openapi.yml
  format: yaml
  label: Ethernovia My Download API
  slug: ethernovia-my-download-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ethernovia/refs/heads/main/openapi/ethernovia-my-download-api-openapi.yml
- filename: ethernovia-upload-file-api-openapi.yml
  format: yaml
  label: Ethernovia Upload - File API
  slug: ethernovia-upload-file-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ethernovia/refs/heads/main/openapi/ethernovia-upload-file-api-openapi.yml
- filename: ethernovia-users-permissions-auth-api-openapi.yml
  format: yaml
  label: Ethernovia Users-Permissions - Auth API
  slug: ethernovia-users-permissions-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ethernovia/refs/heads/main/openapi/ethernovia-users-permissions-auth-api-openapi.yml
- filename: ethernovia-users-permissions-users-roles-api-openapi.yml
  format: yaml
  label: Ethernovia Users-Permissions - Users & Roles API
  slug: ethernovia-users-permissions-users-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ethernovia/refs/heads/main/openapi/ethernovia-users-permissions-users-roles-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ethernovia.com
  spf: true
hosts:
- cert_expires: Oct 10 22:22:28 2026 GMT
  host: www.ethernovia.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 26 15:12:44 2026 GMT
  host: portal.ethernovia.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 26 15:12:35 2026 GMT
  host: portal-admin.ethernovia.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ethernovia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ethernovia, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Ethernovia
provider_slug: ethernovia
slug: ethernovia-domain-security
source_filename: ethernovia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ethernovia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 22:22:28 2026 GMT\n  hsts: null\n- host: portal.ethernovia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 15:12:44 2026 GMT\n  hsts: null\n- host: portal-admin.ethernovia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 15:12:35 2026 GMT\n  hsts: null\ndomains:\n- domain: ethernovia.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ethernovia/refs/heads/main/security/ethernovia-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Semiconductors
- Automotive
- Ethernet
- Networking
- Hardware
- Robotics
- Artificial Intelligence
- Autonomous Vehicles
- Physical AI
---
