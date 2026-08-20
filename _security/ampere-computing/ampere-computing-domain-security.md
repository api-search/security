---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amperecomputing.com
  spf: true
hosts:
- cert_expires: Oct 10 17:18:29 2026 GMT
  chain_certs: 4
  chain_verifies: true
  host: amperecomputing.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 23 21:46:34 2026 GMT
  cert_issuer: C=US, O=GoDaddy.com, CN=GoDaddy TLS Intermediate CA DV - R1v1
  cert_not_before: Jun  8 21:46:34 2026 GMT
  cert_subject: CN=api.amperecomputing.com
  chain_certs: 2
  chain_error: openssl verify code 20 (unable to get local issuer certificate); curl exits 60 without -k, while the control host amperecomputing.com verifies cleanly from the same trust store — the gateway serves an incomplete/unanchored chain
  chain_verifies: false
  host: api.amperecomputing.com
  https: true
  note: Azure API Management gateway (apim-ampere-prod.azure-api.net); not listed in apis.yml because no public API product is published on it
kind: domain-security
layout: security
method: probed
name: Ampere Computing Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ampere Computing, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Ampere Computing
provider_slug: ampere-computing
slug: ampere-computing-domain-security
source_filename: ampere-computing-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: amperecomputing.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 17:18:29 2026 GMT\n  hsts: false\n  chain_certs: 4\n  chain_verifies: true\n- host: api.amperecomputing.com\n  https: true\n  cert_subject: CN=api.amperecomputing.com\n  cert_issuer: 'C=US, O=GoDaddy.com, CN=GoDaddy TLS Intermediate CA DV - R1v1'\n  cert_not_before: Jun  8 21:46:34 2026 GMT\n  cert_expires: Dec 23 21:46:34 2026 GMT\n  chain_certs: 2\n  chain_verifies: false\n  chain_error: 'openssl verify code 20 (unable to get local issuer certificate); curl\n    exits 60 without -k, while the control host amperecomputing.com verifies cleanly\n    from the same trust store — the gateway serves an incomplete/unanchored chain'\n  note: Azure API Management gateway (apim-ampere-prod.azure-api.net); not listed in\n    apis.yml because no public API product is published on it\ndomains:\n\
  - domain: amperecomputing.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ampere-computing/refs/heads/main/security/ampere-computing-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Semiconductors
- Processors
- Cloud Infrastructure
- Arm64
- AI Inference
- Edge Computing
- Compute Hardware
- Open-Source
---
