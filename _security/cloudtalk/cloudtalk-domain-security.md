---
api_specs:
- filename: cloudtalk-agents-api-openapi.yml
  format: yaml
  label: CloudTalk Agents API
  slug: cloudtalk-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudtalk/refs/heads/main/openapi/cloudtalk-agents-api-openapi.yml
- filename: cloudtalk-bulks-api-openapi.yml
  format: yaml
  label: CloudTalk Bulks API
  slug: cloudtalk-bulks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudtalk/refs/heads/main/openapi/cloudtalk-bulks-api-openapi.yml
- filename: cloudtalk-calls-api-openapi.yml
  format: yaml
  label: CloudTalk Calls API
  slug: cloudtalk-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudtalk/refs/heads/main/openapi/cloudtalk-calls-api-openapi.yml
- filename: cloudtalk-campaigns-api-openapi.yml
  format: yaml
  label: CloudTalk Campaigns API
  slug: cloudtalk-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudtalk/refs/heads/main/openapi/cloudtalk-campaigns-api-openapi.yml
- filename: cloudtalk-contacts-api-openapi.yml
  format: yaml
  label: CloudTalk Contacts API
  slug: cloudtalk-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudtalk/refs/heads/main/openapi/cloudtalk-contacts-api-openapi.yml
- filename: cloudtalk-conversation-intelligence-api-openapi.yml
  format: yaml
  label: CloudTalk Conversation Intelligence API
  slug: cloudtalk-conversation-intelligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudtalk/refs/heads/main/openapi/cloudtalk-conversation-intelligence-api-openapi.yml
- filename: cloudtalk-cuecard-api-openapi.yml
  format: yaml
  label: CloudTalk CueCard API
  slug: cloudtalk-cuecard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudtalk/refs/heads/main/openapi/cloudtalk-cuecard-api-openapi.yml
- filename: cloudtalk-groups-api-openapi.yml
  format: yaml
  label: CloudTalk Groups API
  slug: cloudtalk-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudtalk/refs/heads/main/openapi/cloudtalk-groups-api-openapi.yml
- filename: cloudtalk-numbers-api-openapi.yml
  format: yaml
  label: CloudTalk Numbers API
  slug: cloudtalk-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudtalk/refs/heads/main/openapi/cloudtalk-numbers-api-openapi.yml
- filename: cloudtalk-other-api-openapi.yml
  format: yaml
  label: CloudTalk Other API
  slug: cloudtalk-other-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudtalk/refs/heads/main/openapi/cloudtalk-other-api-openapi.yml
- filename: cloudtalk-sms-api-openapi.yml
  format: yaml
  label: CloudTalk Sms API
  slug: cloudtalk-sms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudtalk/refs/heads/main/openapi/cloudtalk-sms-api-openapi.yml
- filename: cloudtalk-tags-api-openapi.yml
  format: yaml
  label: CloudTalk Tags API
  slug: cloudtalk-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudtalk/refs/heads/main/openapi/cloudtalk-tags-api-openapi.yml
- filename: cloudtalk-voiceagent-api-openapi.yml
  format: yaml
  label: CloudTalk VoiceAgent API
  slug: cloudtalk-voiceagent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudtalk/refs/heads/main/openapi/cloudtalk-voiceagent-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "awstrust.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "globalsign.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: cloudtalk.io
  spf: true
hosts:
- cert_expires: Sep 18 21:32:58 2026 GMT
  host: www.cloudtalk.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 21:32:58 2026 GMT
  host: my.cloudtalk.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cloudtalk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CloudTalk, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: CloudTalk
provider_slug: cloudtalk
slug: cloudtalk-domain-security
source_filename: cloudtalk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cloudtalk.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 21:32:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: my.cloudtalk.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 21:32:58 2026 GMT\n  hsts: null\ndomains:\n- domain: cloudtalk.io\n  dnssec: true\n  caa:\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"globalsign.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudtalk/refs/heads/main/security/cloudtalk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Communications
- Voice
- VoIP
- Call Center
- Contact Center
- CCaaS
- Telephony
- SMS
- Conversation Intelligence
---
