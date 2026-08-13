---
api_specs:
- filename: egym-mms-api-v2-openapi.yml
  format: yaml
  label: EGYM MMS API V2
  slug: mms-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/egym/refs/heads/main/openapi/egym-mms-api-v2-openapi.yml
- filename: egym-mms-api-v1-openapi.yml
  format: yaml
  label: EGYM MMS API v1
  slug: mms-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/egym/refs/heads/main/openapi/egym-mms-api-v1-openapi.yml
- filename: egym-data-hub-openapi.yml
  format: yaml
  label: EGYM Data Hub API
  slug: data-hub
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/egym/refs/heads/main/openapi/egym-data-hub-openapi.yml
- filename: egym-data-export-openapi.yml
  format: yaml
  label: EGYM Data Export API
  slug: data-export
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/egym/refs/heads/main/openapi/egym-data-export-openapi.yml
- filename: egym-equipment-vendor-standalone-openapi.yml
  format: yaml
  label: EGYM Equipment Vendor API (standalone clients)
  slug: equipment-vendor-standalone
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/egym/refs/heads/main/openapi/egym-equipment-vendor-standalone-openapi.yml
- filename: egym-equipment-vendor-server-openapi.yml
  format: yaml
  label: EGYM Equipment Vendor API (server-to-server)
  slug: equipment-vendor-server
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/egym/refs/heads/main/openapi/egym-equipment-vendor-server-openapi.yml
- filename: egym-user-connect-openapi.yml
  format: yaml
  label: EGYM User Connect API
  slug: user-connect
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/egym/refs/heads/main/openapi/egym-user-connect-openapi.yml
- filename: egym-canonical-groupx-classes-openapi.yml
  format: yaml
  label: EGYM Canonical GroupX Classes API (blueprint)
  slug: canonical-groupx-classes
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/egym/refs/heads/main/openapi/egym-canonical-groupx-classes-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:security-caa@egym.com"
  - 0 issue "pki.goog"
  - 0 issue "digicert.com"
  - 0 iodef "mailto:it-infrastructure-team@egym.com"
  - 0 issuewild "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: egym.com
  spf: true
hosts:
- cert_expires: Sep 14 13:04:13 2026 GMT
  host: egym.com
  hsts: true
  hsts_max_age: 1000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 16:14:44 2026 GMT
  host: developer.egym.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 15 12:14:57 2026 GMT
  host: mms.api.egym.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Egym Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EGYM, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: EGYM
provider_slug: egym
slug: egym-domain-security
source_filename: egym-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: egym.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 13:04:13 2026 GMT\n  hsts: true\n  hsts_max_age: 1000\n- host: developer.egym.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 16:14:44 2026 GMT\n  hsts: false\n- host: mms.api.egym.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 12:14:57 2026 GMT\n  hsts: null\ndomains:\n- domain: egym.com\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:security-caa@egym.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"digicert.com\"\n  - 0 iodef \"mailto:it-infrastructure-team@egym.com\"\n  - 0 issuewild \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/egym/refs/heads/main/security/egym-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Fitness
- Health
- Wellness
- Corporate Wellness
- Connected Equipment
- Gym Management
- Member Management
- Check-In
- Measurements
- Workouts
- Analytics
- Webhooks
- Germany
---
