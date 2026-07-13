---
api_specs:
- filename: apache-openmeetings-rest-api.json
  format: json
  label: Apache OpenMeetings REST API
  slug: apache-openmeetings-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-openmeetings/refs/heads/main/openapi/apache-openmeetings-rest-api.json
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 iodef "mailto:root@apache.org"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: apache.org
  spf: true
hosts:
- cert_expires: Aug 24 23:33:10 2026 GMT
  host: openmeetings.apache.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Apache Openmeetings Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apache OpenMeetings, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Apache OpenMeetings
provider_slug: apache-openmeetings
slug: apache-openmeetings-domain-security
source_filename: apache-openmeetings-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: openmeetings.apache.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 23:33:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: apache.org\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 iodef \"mailto:root@apache.org\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apache-openmeetings/refs/heads/main/security/apache-openmeetings-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Collaboration
- Video Conferencing
- Web Conferencing
- Whiteboard
- Apache
- Open Source
- Conferencing
---
