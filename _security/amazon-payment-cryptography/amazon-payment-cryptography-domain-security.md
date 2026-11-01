---
api_specs:
- filename: amazon-payment-cryptography-payment-cryptography-control-plane-api-openapi.yml
  format: yaml
  label: Amazon Payment Cryptography Payment Cryptography Control Plane API
  slug: amazon-payment-cryptography-payment-cryptography-control-plane-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-payment-cryptography/openapi/amazon-payment-cryptography-payment-cryptography-control-plane-api-openapi.yml
- filename: amazon-payment-cryptography-default-key-replication-region-api-openapi.yml
  format: yaml
  label: Amazon Payment Cryptography Payment Cryptography Default Key Replication Region API
  slug: amazon-payment-cryptography-default-key-replication-region-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-payment-cryptography/openapi/amazon-payment-cryptography-default-key-replication-region-api-openapi.yml
- filename: amazon-payment-cryptography-operations-api-openapi.yml
  format: yaml
  label: Amazon Payment Cryptography Payment Cryptography Operations API
  slug: amazon-payment-cryptography-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-payment-cryptography/openapi/amazon-payment-cryptography-operations-api-openapi.yml
- filename: amazon-payment-cryptography-resource-policy-api-openapi.yml
  format: yaml
  label: Amazon Payment Cryptography Payment Cryptography Resource Policy API
  slug: amazon-payment-cryptography-resource-policy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-payment-cryptography/openapi/amazon-payment-cryptography-resource-policy-api-openapi.yml
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
- host: controlplane.payment-cryptography.amazonaws.com
  https: false
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Amazon Payment Cryptography Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amazon Payment Cryptography, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Amazon Payment Cryptography
provider_slug: amazon-payment-cryptography
slug: amazon-payment-cryptography-domain-security
source_filename: amazon-payment-cryptography-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: controlplane.payment-cryptography.amazonaws.com\n  https: false\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: amazonaws.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/amazon-payment-cryptography/security/amazon-payment-cryptography-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cryptography
- Financial Services
- Payment Processing
- PCI
---
