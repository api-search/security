---
api_specs:
- filename: quenza-archiveclient-api-openapi.yml
  format: yaml
  label: Quenza ArchiveClient API
  slug: quenza-archiveclient-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quenza/refs/heads/main/openapi/quenza-archiveclient-api-openapi.yml
- filename: quenza-attachgroupmembers-api-openapi.yml
  format: yaml
  label: Quenza AttachGroupMembers API
  slug: quenza-attachgroupmembers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quenza/refs/heads/main/openapi/quenza-attachgroupmembers-api-openapi.yml
- filename: quenza-clients-api-openapi.yml
  format: yaml
  label: Quenza Clients API
  slug: quenza-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quenza/refs/heads/main/openapi/quenza-clients-api-openapi.yml
- filename: quenza-createclient-api-openapi.yml
  format: yaml
  label: Quenza CreateClient API
  slug: quenza-createclient-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quenza/refs/heads/main/openapi/quenza-createclient-api-openapi.yml
- filename: quenza-creategroup-api-openapi.yml
  format: yaml
  label: Quenza CreateGroup API
  slug: quenza-creategroup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quenza/refs/heads/main/openapi/quenza-creategroup-api-openapi.yml
- filename: quenza-createmember-api-openapi.yml
  format: yaml
  label: Quenza CreateMember API
  slug: quenza-createmember-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quenza/refs/heads/main/openapi/quenza-createmember-api-openapi.yml
- filename: quenza-groups-api-openapi.yml
  format: yaml
  label: Quenza Groups API
  slug: quenza-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quenza/refs/heads/main/openapi/quenza-groups-api-openapi.yml
- filename: quenza-listclient-api-openapi.yml
  format: yaml
  label: Quenza ListClient API
  slug: quenza-listclient-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quenza/refs/heads/main/openapi/quenza-listclient-api-openapi.yml
- filename: quenza-listmember-api-openapi.yml
  format: yaml
  label: Quenza ListMember API
  slug: quenza-listmember-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quenza/refs/heads/main/openapi/quenza-listmember-api-openapi.yml
- filename: quenza-listtask-api-openapi.yml
  format: yaml
  label: Quenza ListTask API
  slug: quenza-listtask-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quenza/refs/heads/main/openapi/quenza-listtask-api-openapi.yml
- filename: quenza-members-api-openapi.yml
  format: yaml
  label: Quenza Members API
  slug: quenza-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quenza/refs/heads/main/openapi/quenza-members-api-openapi.yml
- filename: quenza-showclient-api-openapi.yml
  format: yaml
  label: Quenza ShowClient API
  slug: quenza-showclient-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quenza/refs/heads/main/openapi/quenza-showclient-api-openapi.yml
- filename: quenza-tasks-api-openapi.yml
  format: yaml
  label: Quenza Tasks API
  slug: quenza-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quenza/refs/heads/main/openapi/quenza-tasks-api-openapi.yml
- filename: quenza-unarchiveclient-api-openapi.yml
  format: yaml
  label: Quenza UnarchiveClient API
  slug: quenza-unarchiveclient-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quenza/refs/heads/main/openapi/quenza-unarchiveclient-api-openapi.yml
- filename: quenza-updateclient-api-openapi.yml
  format: yaml
  label: Quenza UpdateClient API
  slug: quenza-updateclient-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quenza/refs/heads/main/openapi/quenza-updateclient-api-openapi.yml
- filename: quenza-updatemember-api-openapi.yml
  format: yaml
  label: Quenza UpdateMember API
  slug: quenza-updatemember-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quenza/refs/heads/main/openapi/quenza-updatemember-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: quenza.com
  spf: true
hosts:
- cert_expires: Aug 17 18:32:49 2026 GMT
  host: quenza.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 22:47:47 2026 GMT
  host: developers.quenza.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Quenza Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Quenza, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Quenza
provider_slug: quenza
slug: quenza-domain-security
source_filename: quenza-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: quenza.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 18:32:49 2026 GMT\n  hsts: false\n- host: developers.quenza.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 22:47:47 2026 GMT\n  hsts: false\ndomains:\n- domain: quenza.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quenza/refs/heads/main/security/quenza-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Coaching
- Therapy
- Client Engagement
- Digital Health
- Mental Health
- Practice Management
- Positive Psychology
---
