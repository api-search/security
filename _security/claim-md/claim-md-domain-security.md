---
api_specs:
- filename: claim-md-openapi.yml
  format: yaml
  label: Claim.MD Claim Submission API
  slug: claim-submission
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/claim-md/refs/heads/main/openapi/claim-md-openapi.yml
- filename: claim-md-openapi.yml
  format: yaml
  label: Claim.MD Claim Status API
  slug: claim-status
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/claim-md/refs/heads/main/openapi/claim-md-openapi.yml
- filename: claim-md-openapi.yml
  format: yaml
  label: Claim.MD ERA / Remits API
  slug: era-remits
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/claim-md/refs/heads/main/openapi/claim-md-openapi.yml
- filename: claim-md-openapi.yml
  format: yaml
  label: Claim.MD Eligibility API
  slug: eligibility
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/claim-md/refs/heads/main/openapi/claim-md-openapi.yml
- filename: claim-md-openapi.yml
  format: yaml
  label: Claim.MD Responses & Files API
  slug: responses-files
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/claim-md/refs/heads/main/openapi/claim-md-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "entrust.net"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: claim.md
  spf: true
hosts:
- cert_expires: Mar 16 23:59:59 2027 GMT
  host: www.claim.md
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 06:14:02 2026 GMT
  host: docs.claim.md
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 23 23:59:59 2027 GMT
  host: svc.claim.md
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Claim Md Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Claim.MD, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Claim.MD
provider_slug: claim-md
slug: claim-md-domain-security
source_filename: claim-md-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.claim.md\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 16 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.claim.md\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 06:14:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: svc.claim.md\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 23 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: claim.md\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"entrust.net\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/claim-md/refs/heads/main/security/claim-md-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Healthcare
- Medical Claims
- Clearinghouse
- EDI
- X12
- Revenue Cycle
---
