---
api_specs:
- filename: panopto-accessibility-api-openapi.yml
  format: yaml
  label: Panopto Accessibility API
  slug: panopto-accessibility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/panopto/refs/heads/main/openapi/panopto-accessibility-api-openapi.yml
- filename: panopto-auth-api-openapi.yml
  format: yaml
  label: Panopto Auth API
  slug: panopto-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/panopto/refs/heads/main/openapi/panopto-auth-api-openapi.yml
- filename: panopto-captionproviders-api-openapi.yml
  format: yaml
  label: Panopto CaptionProviders API
  slug: panopto-captionproviders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/panopto/refs/heads/main/openapi/panopto-captionproviders-api-openapi.yml
- filename: panopto-folders-api-openapi.yml
  format: yaml
  label: Panopto Folders API
  slug: panopto-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/panopto/refs/heads/main/openapi/panopto-folders-api-openapi.yml
- filename: panopto-groups-api-openapi.yml
  format: yaml
  label: Panopto Groups API
  slug: panopto-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/panopto/refs/heads/main/openapi/panopto-groups-api-openapi.yml
- filename: panopto-playlists-api-openapi.yml
  format: yaml
  label: Panopto Playlists API
  slug: panopto-playlists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/panopto/refs/heads/main/openapi/panopto-playlists-api-openapi.yml
- filename: panopto-remoterecorderapi-api-openapi.yml
  format: yaml
  label: Panopto RemoteRecorderAPI API
  slug: panopto-remoterecorderapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/panopto/refs/heads/main/openapi/panopto-remoterecorderapi-api-openapi.yml
- filename: panopto-remoterecorders-api-openapi.yml
  format: yaml
  label: Panopto RemoteRecorders API
  slug: panopto-remoterecorders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/panopto/refs/heads/main/openapi/panopto-remoterecorders-api-openapi.yml
- filename: panopto-reports-api-openapi.yml
  format: yaml
  label: Panopto Reports API
  slug: panopto-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/panopto/refs/heads/main/openapi/panopto-reports-api-openapi.yml
- filename: panopto-scheduledrecordings-api-openapi.yml
  format: yaml
  label: Panopto ScheduledRecordings API
  slug: panopto-scheduledrecordings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/panopto/refs/heads/main/openapi/panopto-scheduledrecordings-api-openapi.yml
- filename: panopto-searchindexsyncupdates-api-openapi.yml
  format: yaml
  label: Panopto SearchIndexSyncUpdates API
  slug: panopto-searchindexsyncupdates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/panopto/refs/heads/main/openapi/panopto-searchindexsyncupdates-api-openapi.yml
- filename: panopto-sessions-api-openapi.yml
  format: yaml
  label: Panopto Sessions API
  slug: panopto-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/panopto/refs/heads/main/openapi/panopto-sessions-api-openapi.yml
- filename: panopto-streams-api-openapi.yml
  format: yaml
  label: Panopto Streams API
  slug: panopto-streams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/panopto/refs/heads/main/openapi/panopto-streams-api-openapi.yml
- filename: panopto-tags-api-openapi.yml
  format: yaml
  label: Panopto Tags API
  slug: panopto-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/panopto/refs/heads/main/openapi/panopto-tags-api-openapi.yml
- filename: panopto-users-api-openapi.yml
  format: yaml
  label: Panopto Users API
  slug: panopto-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/panopto/refs/heads/main/openapi/panopto-users-api-openapi.yml
- filename: panopto-xfpuserprofiles-api-openapi.yml
  format: yaml
  label: Panopto XfpUserProfiles API
  slug: panopto-xfpuserprofiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/panopto/refs/heads/main/openapi/panopto-xfpuserprofiles-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "awstrust.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "godaddy.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: panopto.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: panopto.com)
  spf: false
hosts:
- cert_expires: Sep  2 14:09:57 2026 GMT
  host: www.panopto.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: support.panopto.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get local issuer certificate (_ssl.c:1082)'
- host: <panoptoserverurl>(i.e. example.hosted.panopto.com)
  https: false
kind: domain-security
layout: security
method: probed
name: Panopto Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Panopto, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Panopto
provider_slug: panopto
slug: panopto-domain-security
source_filename: panopto-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.panopto.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 14:09:57 2026 GMT\n  hsts: false\n- host: support.panopto.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get\n    local issuer certificate (_ssl.c:1082)'\n  hsts: null\n- host: <panoptoserverurl>(i.e. example.hosted.panopto.com)\n  https: false\ndomains:\n- domain: panopto.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"godaddy.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: panopto.com)\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/panopto/refs/heads/main/security/panopto-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Video Management
- Education Technology
- Enterprise Video
- Recording
- Learning Management
- Video Analytics
- Content Management
---
