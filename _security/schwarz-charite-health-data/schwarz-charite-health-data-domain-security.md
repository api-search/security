---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: schwarz-digits.de
  spf: true
hosts:
- cert_expires: Nov  1 23:56:54 2026 GMT
  host: schwarz-digits.de
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Schwarz Charite Health Data Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Schwarz Charite Health Data, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Schwarz Charite Health Data
provider_slug: schwarz-charite-health-data
slug: schwarz-charite-health-data-domain-security
source_filename: schwarz-charite-health-data-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: schwarz-digits.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 23:56:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: schwarz-digits.de\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/schwarz-charite-health-data/refs/heads/main/security/schwarz-charite-health-data-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Health Data
- Healthcare
- Clinical Data Repository
- openEHR
- Interoperability
- HL7 FHIR
- Data Sovereignty
- Cloud
- Germany
- Joint Venture
---
