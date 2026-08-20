---
api_specs:
- filename: certifid-accountverifications-api-openapi.yml
  format: yaml
  label: CertifID Account Verifications API
  slug: certifid-accountverifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/certifid/refs/heads/main/openapi/certifid-accountverifications-api-openapi.yml
- filename: certifid-banklookup-api-openapi.yml
  format: yaml
  label: CertifID Bank Lookup API
  slug: certifid-banklookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/certifid/refs/heads/main/openapi/certifid-banklookup-api-openapi.yml
- filename: certifid-collectrequest-api-openapi.yml
  format: yaml
  label: CertifID Collect Request API
  slug: certifid-collectrequest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/certifid/refs/heads/main/openapi/certifid-collectrequest-api-openapi.yml
- filename: certifid-confirmrequest-api-openapi.yml
  format: yaml
  label: CertifID Confirm Request API
  slug: certifid-confirmrequest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/certifid/refs/heads/main/openapi/certifid-confirmrequest-api-openapi.yml
- filename: certifid-disbursements-api-openapi.yml
  format: yaml
  label: CertifID Disbursements API
  slug: certifid-disbursements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/certifid/refs/heads/main/openapi/certifid-disbursements-api-openapi.yml
- filename: certifid-identityrequest-api-openapi.yml
  format: yaml
  label: CertifID Identity Request API
  slug: certifid-identityrequest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/certifid/refs/heads/main/openapi/certifid-identityrequest-api-openapi.yml
- filename: certifid-integration-api-openapi.yml
  format: yaml
  label: CertifID Integration API
  slug: certifid-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/certifid/refs/heads/main/openapi/certifid-integration-api-openapi.yml
- filename: certifid-lenders-api-openapi.yml
  format: yaml
  label: CertifID Lenders API
  slug: certifid-lenders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/certifid/refs/heads/main/openapi/certifid-lenders-api-openapi.yml
- filename: certifid-location-api-openapi.yml
  format: yaml
  label: CertifID Location API
  slug: certifid-location-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/certifid/refs/heads/main/openapi/certifid-location-api-openapi.yml
- filename: certifid-payoffordering-api-openapi.yml
  format: yaml
  label: CertifID Payoff Ordering API
  slug: certifid-payoffordering-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/certifid/refs/heads/main/openapi/certifid-payoffordering-api-openapi.yml
- filename: certifid-sendrequest-api-openapi.yml
  format: yaml
  label: CertifID Send Request API
  slug: certifid-sendrequest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/certifid/refs/heads/main/openapi/certifid-sendrequest-api-openapi.yml
- filename: certifid-test-api-openapi.yml
  format: yaml
  label: CertifID Test API
  slug: certifid-test-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/certifid/refs/heads/main/openapi/certifid-test-api-openapi.yml
- filename: certifid-underwriter-api-openapi.yml
  format: yaml
  label: CertifID Underwriter API
  slug: certifid-underwriter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/certifid/refs/heads/main/openapi/certifid-underwriter-api-openapi.yml
- filename: certifid-users-api-openapi.yml
  format: yaml
  label: CertifID Users API
  slug: certifid-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/certifid/refs/heads/main/openapi/certifid-users-api-openapi.yml
- filename: certifid-wiringinstructions-api-openapi.yml
  format: yaml
  label: CertifID Wiring Instructions API
  slug: certifid-wiringinstructions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/certifid/refs/heads/main/openapi/certifid-wiringinstructions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: certifid.com
  spf: true
hosts:
- cert_expires: Oct 30 05:59:32 2026 GMT
  host: www.certifid.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 28 05:34:53 2026 GMT
  host: api.certifid.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Certifid Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CertifID, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: CertifID
provider_slug: certifid
slug: certifid-domain-security
source_filename: certifid-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.certifid.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 05:59:32 2026 GMT\n  hsts: true\n  hsts_max_age: 0\n- host: api.certifid.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 05:34:53 2026 GMT\n  hsts: null\ndomains:\n- domain: certifid.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/certifid/refs/heads/main/security/certifid-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Wire Fraud Prevention
- Real-Estate
- Title Insurance
- Identity Verification
- Business Verification
- Payments
- Fraud Prevention
- Escrow and Settlement
- Financial-Services
- Security
---
