---
api_specs:
- filename: nexhealth-openapi-original.json
  format: json
  label: NexHealth Synchronizer API
  slug: nexhealth-synchronizer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexhealth/refs/heads/main/openapi/nexhealth-openapi-original.json
description: ''
domains:
- caa:
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: nexhealth.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: nexhealth.info
  spf: true
hosts:
- cert_expires: Oct 14 16:00:33 2026 GMT
  host: www.nexhealth.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 10:01:45 2026 GMT
  host: nexhealth.info
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nexhealth Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NexHealth, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: NexHealth
provider_slug: nexhealth
slug: nexhealth-domain-security
source_filename: nexhealth-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nexhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 16:00:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: nexhealth.info\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 10:01:45 2026 GMT\n  hsts: null\ndomains:\n- domain: nexhealth.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: nexhealth.info\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nexhealth/refs/heads/main/security/nexhealth-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Healthcare
- EHR
- Practice Management
- Scheduling
- Appointments
- Dental
- Patients
- Health Records
- Insurance
- Webhooks
---
