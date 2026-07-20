---
api_specs:
- filename: schema
  format: yaml
  label: Jamf Pro API
  slug: jamf-pro-api
  spec_type: OpenAPI
  url: https://your-instance.jamfcloud.com/api/schema
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: jamf.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: jamfcloud.com
  spf: true
hosts:
- cert_expires: Mar 12 23:59:59 2027 GMT
  host: www.jamf.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 00:51:55 2026 GMT
  host: developer.jamf.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 25 23:59:59 2027 GMT
  host: your-instance.jamfcloud.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jamf Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for JAMF, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: JAMF
provider_slug: jamf
slug: jamf-domain-security
source_filename: jamf-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.jamf.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 12 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.jamf.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 00:51:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: your-instance.jamfcloud.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 25 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: jamf.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: jamfcloud.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jamf/refs/heads/main/security/jamf-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Apple Device Management
- MDM
- Endpoint Security
- Mobile Device Management
- IT Operations
- Identity
- Compliance
- Developer Tools
- Enterprise
---
