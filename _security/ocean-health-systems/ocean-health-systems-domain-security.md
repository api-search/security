---
api_specs:
- filename: ocean-health-systems-ckm-rest-api-openapi.json
  format: json
  label: CKM REST API
  slug: ckm-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ocean-health-systems/refs/heads/main/openapi/ocean-health-systems-ckm-rest-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: oceanhealthsystems.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: openehr.org
  spf: true
hosts:
- cert_expires: Nov 20 11:00:41 2026 GMT
  host: oceanhealthsystems.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 19:15:14 2026 GMT
  host: ckm.openehr.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ocean Health Systems Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ocean Health Systems, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Ocean Health Systems
provider_slug: ocean-health-systems
slug: ocean-health-systems-domain-security
source_filename: ocean-health-systems-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: oceanhealthsystems.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 11:00:41 2026 GMT\n  hsts: false\n- host: ckm.openehr.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 19:15:14 2026 GMT\n  hsts: false\ndomains:\n- domain: oceanhealthsystems.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: openehr.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ocean-health-systems/refs/heads/main/security/ocean-health-systems-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Health
- Healthcare
- Electronic Health Records
- openEHR
- Clinical Data
- Clinical Knowledge Management
- Interoperability
- Health Informatics
- Terminology
- Archetypes
- Infection Prevention
- Immunisation
---
