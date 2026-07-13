---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: TenantCloud API
  slug: tenantcloud-api
  spec_type: OpenAPI
  url: https://docs.api.tenantcloud.com/
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: tenantcloud.com
  spf: true
hosts:
- host: docs.api.tenantcloud.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''docs.api.te'
- cert_expires: Jan 21 23:59:59 2027 GMT
  host: api.tenantcloud.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tenantcloud Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TenantCloud, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: TenantCloud
provider_slug: tenantcloud
slug: tenantcloud-domain-security
source_filename: tenantcloud-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.api.tenantcloud.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''docs.api.te'\n  hsts: null\n- host: api.tenantcloud.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tenantcloud.com\n  dnssec: true\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tenantcloud/refs/heads/main/security/tenantcloud-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Property Management
- Real Estate
- Rental
- Tenant Management
- Lease Management
- Maintenance
- Accounting
- Rent Payments
---
