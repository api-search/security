---
api_specs:
- filename: openapi.json
  format: json
  label: Red Hat Subscription Management API
  slug: subscription-management-api
  spec_type: OpenAPI
  url: https://api.access.redhat.com/management/v1/openapi.json
- filename: openapi.json
  format: json
  label: Red Hat Insights API
  slug: insights-api
  spec_type: OpenAPI
  url: https://cloud.redhat.com/api/insights/v1/openapi.json
- filename: rhel-security-data-openapi.yml
  format: yaml
  label: Red Hat Security Data API
  slug: security-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rhel/refs/heads/main/openapi/rhel-security-data-openapi.yml
- filename: openapi.json
  format: json
  label: Red Hat Insights Compliance API
  slug: compliance-api
  spec_type: OpenAPI
  url: https://console.redhat.com/api/compliance/v2/openapi.json
- filename: openapi.json
  format: json
  label: Red Hat Insights Vulnerability API
  slug: vulnerability-api
  spec_type: OpenAPI
  url: https://console.redhat.com/api/vulnerability/v1/openapi.json
- filename: openapi.json
  format: json
  label: Red Hat Insights Patch API
  slug: patch-api
  spec_type: OpenAPI
  url: https://console.redhat.com/api/patch/v3/openapi.json
- filename: openapi.json
  format: json
  label: Red Hat Insights Host Inventory API
  slug: inventory-api
  spec_type: OpenAPI
  url: https://console.redhat.com/api/inventory/v1/openapi.json
- filename: openapi.json
  format: json
  label: Red Hat Insights Remediations API
  slug: remediations-api
  spec_type: OpenAPI
  url: https://console.redhat.com/api/remediations/v1/openapi.json
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  - 0 iodef "mailto:it-cert-admin@redhat.com"
  - 0 issue "amazontrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: redhat.com
  spf: true
hosts:
- cert_expires: Oct 27 23:59:59 2026 GMT
  host: access.redhat.com
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 10 23:59:59 2026 GMT
  host: www.redhat.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 16 23:59:59 2027 GMT
  host: api.access.redhat.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rhel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Red Hat Enterprise Linux, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Red Hat Enterprise Linux
provider_slug: rhel
slug: rhel-domain-security
source_filename: rhel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: access.redhat.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\n- host: www.redhat.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.access.redhat.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 16 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: redhat.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  - 0 iodef \"mailto:it-cert-admin@redhat.com\"\n  - 0 issue \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rhel/refs/heads/main/security/rhel-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Automation
- Compliance
- Enterprise
- Linux
- Operating System
- Red Hat
- RHEL
- Security
- Subscription Management
- Vulnerability Management
---
