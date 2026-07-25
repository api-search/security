---
api_specs:
- filename: amazon-signer-revocations-signaturetimestamp-platformid-profileversionarn-jobarn-certificatehashes-api-openapi.yml
  format: yaml
  label: Amazon Signer Revocations#signatureTimestamp&platformId&profileVersionArn&jobArn&certificateHashes API
  slug: amazon-signer-revocations-signaturetimestamp-platformid-profileversionarn-jobarn-certificatehashes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-signer/refs/heads/main/openapi/amazon-signer-revocations-signaturetimestamp-platformid-profileversionarn-jobarn-certificatehashes-api-openapi.yml
- filename: amazon-signer-signing-jobs-api-openapi.yml
  format: yaml
  label: Amazon Signer Signing Jobs API
  slug: amazon-signer-signing-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-signer/refs/heads/main/openapi/amazon-signer-signing-jobs-api-openapi.yml
- filename: amazon-signer-signing-platforms-api-openapi.yml
  format: yaml
  label: Amazon Signer Signing Platforms API
  slug: amazon-signer-signing-platforms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-signer/refs/heads/main/openapi/amazon-signer-signing-platforms-api-openapi.yml
- filename: amazon-signer-signing-profiles-api-openapi.yml
  format: yaml
  label: Amazon Signer Signing Profiles API
  slug: amazon-signer-signing-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-signer/refs/heads/main/openapi/amazon-signer-signing-profiles-api-openapi.yml
- filename: amazon-signer-tags-api-openapi.yml
  format: yaml
  label: Amazon Signer Tags API
  slug: amazon-signer-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-signer/refs/heads/main/openapi/amazon-signer-tags-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amazon.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amazonaws.com
  spf: true
hosts:
- cert_expires: Oct 17 23:59:59 2026 GMT
  host: aws.amazon.com
  hsts: true
  hsts_max_age: 47304000
  https: true
  tls_version: TLSv1.3
- host: signer.amazonaws.com
  https: false
kind: domain-security
layout: security
method: probed
name: Amazon Signer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amazon Signer, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Amazon Signer
provider_slug: amazon-signer
slug: amazon-signer-domain-security
source_filename: amazon-signer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: signer.amazonaws.com\n  https: false\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: amazonaws.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-signer/refs/heads/main/security/amazon-signer-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Code Signing
- IoT
- Lambda
- Security
---
