---
api_specs:
- filename: sift-openapi.yml
  format: yaml
  label: Sift Events API
  slug: sift-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sift/refs/heads/main/openapi/sift-openapi.yml
- filename: sift-openapi.yml
  format: yaml
  label: Sift Score API
  slug: sift-score-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sift/refs/heads/main/openapi/sift-openapi.yml
- filename: sift-openapi.yml
  format: yaml
  label: Sift Decisions API
  slug: sift-decisions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sift/refs/heads/main/openapi/sift-openapi.yml
- filename: sift-openapi.yml
  format: yaml
  label: Sift Workflow Status API
  slug: sift-workflow-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sift/refs/heads/main/openapi/sift-openapi.yml
- filename: sift-openapi.yml
  format: yaml
  label: Sift Labels API
  slug: sift-labels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sift/refs/heads/main/openapi/sift-openapi.yml
- filename: sift-openapi.yml
  format: yaml
  label: Sift Verification API
  slug: sift-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sift/refs/heads/main/openapi/sift-openapi.yml
- filename: sift-openapi.yml
  format: yaml
  label: Sift PSP Merchant Management API
  slug: sift-psp-merchant-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sift/refs/heads/main/openapi/sift-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sift.com
  spf: false
- caa:
  - CNAME to developers.prod.gcp.sift.com (GCP-hosted)
  dmarc: false
  dnssec: false
  domain: developers.sift.com
  note: developers.sift.com resolves via CNAME to developers.prod.gcp.sift.com; DMARC/SPF are set at the sift.com organizational domain.
  spf: false
- caa:
  - CNAME to public.api.prod.gcp.sift.com (GCP-hosted)
  dmarc: false
  dnssec: false
  domain: api.sift.com
  note: api.sift.com resolves via CNAME to public.api.prod.gcp.sift.com; the API host does not send HSTS but serves TLS 1.3 only.
  spf: false
hosts:
- cert_expires: Sep  6 01:38:22 2026 GMT
  host: sift.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 16 23:59:59 2027 GMT
  host: developers.sift.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_preload: true
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 22 23:59:59 2027 GMT
  host: api.sift.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sift Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sift, probed live across 3 host(s) and 3 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: Sift
provider_slug: sift
slug: sift-domain-security
source_filename: sift-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sift.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 01:38:22 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developers.sift.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 16 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  hsts_preload: true\n- host: api.sift.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 22 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: sift.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n- domain: developers.sift.com\n  dnssec: false\n  caa:\n  - 'CNAME to developers.prod.gcp.sift.com (GCP-hosted)'\n  spf: false\n  dmarc: false\n  note: developers.sift.com resolves via CNAME to developers.prod.gcp.sift.com; DMARC/SPF are set at the sift.com organizational domain.\n- domain: api.sift.com\n\
  \  dnssec: false\n  caa:\n  - 'CNAME to public.api.prod.gcp.sift.com (GCP-hosted)'\n  spf: false\n  dmarc: false\n  note: api.sift.com resolves via CNAME to public.api.prod.gcp.sift.com; the API host does not send HSTS but serves TLS 1.3 only.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sift/refs/heads/main/security/sift-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fraud Detection
- Fraud Prevention
- Risk
- Trust and Safety
- Machine Learning
- Payment Fraud
- Account Takeover
- Chargebacks
- Digital Trust
---
