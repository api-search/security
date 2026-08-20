---
api_specs:
- filename: apache-openmeetings-calendarservice-api-openapi.yml
  format: yaml
  label: Apache OpenMeetings CalendarService API
  slug: apache-openmeetings-calendarservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-openmeetings/refs/heads/main/openapi/apache-openmeetings-calendarservice-api-openapi.yml
- filename: apache-openmeetings-errorservice-api-openapi.yml
  format: yaml
  label: Apache OpenMeetings ErrorService API
  slug: apache-openmeetings-errorservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-openmeetings/refs/heads/main/openapi/apache-openmeetings-errorservice-api-openapi.yml
- filename: apache-openmeetings-fileservice-api-openapi.yml
  format: yaml
  label: Apache OpenMeetings FileService API
  slug: apache-openmeetings-fileservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-openmeetings/refs/heads/main/openapi/apache-openmeetings-fileservice-api-openapi.yml
- filename: apache-openmeetings-groupservice-api-openapi.yml
  format: yaml
  label: Apache OpenMeetings GroupService API
  slug: apache-openmeetings-groupservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-openmeetings/refs/heads/main/openapi/apache-openmeetings-groupservice-api-openapi.yml
- filename: apache-openmeetings-infoservice-api-openapi.yml
  format: yaml
  label: Apache OpenMeetings InfoService API
  slug: apache-openmeetings-infoservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-openmeetings/refs/heads/main/openapi/apache-openmeetings-infoservice-api-openapi.yml
- filename: apache-openmeetings-nettestservice-api-openapi.yml
  format: yaml
  label: Apache OpenMeetings NetTestService API
  slug: apache-openmeetings-nettestservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-openmeetings/refs/heads/main/openapi/apache-openmeetings-nettestservice-api-openapi.yml
- filename: apache-openmeetings-recordingservice-api-openapi.yml
  format: yaml
  label: Apache OpenMeetings RecordingService API
  slug: apache-openmeetings-recordingservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-openmeetings/refs/heads/main/openapi/apache-openmeetings-recordingservice-api-openapi.yml
- filename: apache-openmeetings-roomservice-api-openapi.yml
  format: yaml
  label: Apache OpenMeetings RoomService API
  slug: apache-openmeetings-roomservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-openmeetings/refs/heads/main/openapi/apache-openmeetings-roomservice-api-openapi.yml
- filename: apache-openmeetings-userservice-api-openapi.yml
  format: yaml
  label: Apache OpenMeetings UserService API
  slug: apache-openmeetings-userservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-openmeetings/refs/heads/main/openapi/apache-openmeetings-userservice-api-openapi.yml
- filename: apache-openmeetings-wbservice-api-openapi.yml
  format: yaml
  label: Apache OpenMeetings WbService API
  slug: apache-openmeetings-wbservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-openmeetings/refs/heads/main/openapi/apache-openmeetings-wbservice-api-openapi.yml
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
- Open-Source
- Conferencing
---
