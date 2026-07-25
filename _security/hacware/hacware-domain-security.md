---
api_specs:
- filename: hacware-admin-api-openapi.yml
  format: yaml
  label: Hacware Admin API
  slug: hacware-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hacware/refs/heads/main/openapi/hacware-admin-api-openapi.yml
- filename: hacware-compliance-api-openapi.yml
  format: yaml
  label: Hacware Compliance API
  slug: hacware-compliance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hacware/refs/heads/main/openapi/hacware-compliance-api-openapi.yml
- filename: hacware-compliance-tenant-api-openapi.yml
  format: yaml
  label: Hacware Compliance-Tenant API
  slug: hacware-compliance-tenant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hacware/refs/heads/main/openapi/hacware-compliance-tenant-api-openapi.yml
- filename: hacware-customer-api-openapi.yml
  format: yaml
  label: Hacware Customer API
  slug: hacware-customer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hacware/refs/heads/main/openapi/hacware-customer-api-openapi.yml
- filename: hacware-email-tenant-api-openapi.yml
  format: yaml
  label: Hacware Email-Tenant API
  slug: hacware-email-tenant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hacware/refs/heads/main/openapi/hacware-email-tenant-api-openapi.yml
- filename: hacware-group-api-openapi.yml
  format: yaml
  label: Hacware Group API
  slug: hacware-group-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hacware/refs/heads/main/openapi/hacware-group-api-openapi.yml
- filename: hacware-multi-tenant-api-openapi.yml
  format: yaml
  label: Hacware Multi-Tenant API
  slug: hacware-multi-tenant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hacware/refs/heads/main/openapi/hacware-multi-tenant-api-openapi.yml
- filename: hacware-phishing-api-openapi.yml
  format: yaml
  label: Hacware Phishing API
  slug: hacware-phishing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hacware/refs/heads/main/openapi/hacware-phishing-api-openapi.yml
- filename: hacware-report-api-openapi.yml
  format: yaml
  label: Hacware Report API
  slug: hacware-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hacware/refs/heads/main/openapi/hacware-report-api-openapi.yml
- filename: hacware-training-api-openapi.yml
  format: yaml
  label: Hacware Training API
  slug: hacware-training-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hacware/refs/heads/main/openapi/hacware-training-api-openapi.yml
- filename: hacware-user-api-openapi.yml
  format: yaml
  label: Hacware User API
  slug: hacware-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hacware/refs/heads/main/openapi/hacware-user-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: hacware.com
  spf: true
hosts:
- cert_expires: Jan 19 23:59:59 2027 GMT
  host: hacware.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan 19 23:59:59 2027 GMT
  host: www.hacware.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- host: app.hacware.com
  https: false
kind: domain-security
layout: security
method: probed
name: Hacware Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hacware, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Hacware
provider_slug: hacware
slug: hacware-domain-security
source_filename: hacware-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hacware.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 19 23:59:59 2027 GMT\n  hsts: false\n- host: www.hacware.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 19 23:59:59 2027 GMT\n  hsts: false\n- host: app.hacware.com\n  https: false\ndomains:\n- domain: hacware.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hacware/refs/heads/main/security/hacware-domain-security.yml
summary_line: TLSv1.2 · DNSSEC · DMARC
tags:
- Company
- Security
- Cybersecurity
- Security Awareness
- Phishing
- Training
- Compliance
- Email Security
- Artificial Intelligence
---
