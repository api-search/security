---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: evercontact.com
  spf: true
hosts:
- cert_expires: Oct 28 04:08:48 2026 GMT
  host: www.evercontact.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_issuer: C=US, O=Amazon, CN=Amazon RSA 2048 M01
  cert_sans:
  - b2b-lb.eu-prod.sonysnacloud.net
  cert_subject_cn: b2b-lb.eu-prod.sonysnacloud.net
  finding: The published API base host does not present an Evercontact certificate. DNS resolves to an AWS ELB whose only certificate name is a Sony property (b2b-lb.eu-prod.sonysnacloud.net), so TLS fails for every conforming client and the load balancer answers 403 to everything. Reads as a dangling DNS record on recycled AWS infrastructure. Full probe record in well-known/evercontact-well-known.yml (api_host_finding).
  host: api.evercontact.com
  hsts: null
  http_status_verification_disabled: 403
  https: true
  server_header: awselb/2.0
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''api.evercon'
kind: domain-security
layout: security
method: probed
name: Evercontact Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Evercontact, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Evercontact
provider_slug: evercontact
slug: evercontact-domain-security
source_filename: evercontact-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.evercontact.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 04:08:48 2026 GMT\n  hsts: false\n- host: api.evercontact.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''api.evercon'\n  hsts: null\n  cert_subject_cn: b2b-lb.eu-prod.sonysnacloud.net\n  cert_issuer: 'C=US, O=Amazon, CN=Amazon RSA 2048 M01'\n  cert_sans:\n  - b2b-lb.eu-prod.sonysnacloud.net\n  http_status_verification_disabled: 403\n  server_header: awselb/2.0\n  finding: >-\n    The published API base host does not present an Evercontact certificate. DNS\n    resolves to an AWS ELB whose only certificate name is a Sony property\n    (b2b-lb.eu-prod.sonysnacloud.net), so TLS fails for every conforming client and\n    the load balancer answers 403 to everything. Reads as\
  \ a dangling DNS record on\n    recycled AWS infrastructure. Full probe record in\n    well-known/evercontact-well-known.yml (api_host_finding).\ndomains:\n- domain: evercontact.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/evercontact/refs/heads/main/security/evercontact-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Contact Management
- Contact Data
- Data Enrichment
- Email
- Signature Parsing
- Data Extraction
- CRM
---
