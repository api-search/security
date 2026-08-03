---
api_specs:
- filename: fortanix-dsm-openapi-original.json
  format: json
  label: Fortanix Data Security Manager REST API
  slug: dsm
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fortanix/refs/heads/main/openapi/fortanix-dsm-openapi-original.json
- filename: fortanix-ccm-openapi-original.json
  format: json
  label: Fortanix Confidential Computing Manager REST API
  slug: ccm
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fortanix/refs/heads/main/openapi/fortanix-ccm-openapi-original.json
- filename: fortanix-armor-key-insight-openapi-original.json
  format: json
  label: Fortanix Armor and Key Insight API
  slug: armor-key-insight
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fortanix/refs/heads/main/openapi/fortanix-armor-key-insight-openapi-original.json
certifications:
- SOC 2
- ISO 27001
- PCI DSS
- FIPS 140-2 Level 3
- CIS Benchmarks
description: ''
kind: trust-center
layout: security
name: Fortanix Trust Center
name_suffix: Trust Center
overview: Fortanix maintains a public trust center documenting SOC 2, ISO 27001, PCI DSS, FIPS 140-2 Level 3, and CIS Benchmarks compliance.
provider_name: Fortanix
provider_slug: fortanix
slug: fortanix-trust-center
source_filename: fortanix-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: searched\nprobe: true\nsource: https://www.fortanix.com/trust-center\nurl: https://www.fortanix.com/trust-center\ncertifications:\n- SOC 2\n- ISO 27001\n- PCI DSS\n- FIPS 140-2 Level 3\n- CIS Benchmarks\nnotes: 'The Fortanix Data Security Manager application runs inside an Intel SGX secure\n  enclave and is a FIPS 140-2 Level 3 validated cryptographic module. The trust center\n  also publishes the Fortanix key-attestation PKI: a publicly available root CA certificate,\n  three certification-policy documents and an audit report, used to prove provenance\n  of keys generated in Fortanix DSM.'\nsecurity_contact: security@fortanix.com\npgp_key: https://www.fortanix.com/trust-center/pgp-key\nevidence:\n- source: https://www.fortanix.com/trust-center\n  http_status: 200\n  fetched: '2026-08-01'\n  keywords:\n  - soc 2\n  - iso 27001\n  - pci dss\n  - fips 140-2 level 3\n  - cis\n- source: https://www.fortanix.com/.well-known/security.txt\n  http_status:\
  \ 200\n  kind: security.txt Policy field points at the trust center\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fortanix/refs/heads/main/security/fortanix-trust-center.yml
summary_line: SOC 2, ISO 27001, PCI DSS, FIPS 140-2 Level 3, CIS Benchmarks
tags:
- Company
- Security
- Encryption
- Key Management
- Cryptography
- Confidential Computing
- HSM
- Data Security
- Post-Quantum
- Secrets Management
trust_url: https://www.fortanix.com/trust-center
---
