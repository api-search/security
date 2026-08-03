---
api_specs:
- filename: threatlocker-portal-openapi-original.json
  format: json
  label: ThreatLocker PortalAPI
  slug: threatlocker-portalapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/threatlocker/refs/heads/main/openapi/threatlocker-portal-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: threatlocker.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: kb.help
  spf: false
hosts:
- cert_expires: Nov 10 23:59:59 2026 GMT
  host: www.threatlocker.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  7 23:59:59 2026 GMT
  host: threatlocker.kb.help
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 26 23:59:59 2026 GMT
  host: portalapi.threatlocker.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Threatlocker Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ThreatLocker, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ThreatLocker
provider_slug: threatlocker
slug: threatlocker-domain-security
source_filename: threatlocker-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.threatlocker.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: threatlocker.kb.help\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 23:59:59 2026 GMT\n  hsts: false\n- host: portalapi.threatlocker.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: threatlocker.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: kb.help\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/threatlocker/refs/heads/main/security/threatlocker-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- cybersecurity
- zero-trust
- endpoint-security
- application-control
- allowlisting
- ransomware-prevention
- privileged-access-management
- network-access-control
- managed-detection-and-response
- device-management
- msp
- compliance
---
