---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mirrorfly.com
  spf: true
hosts:
- cert_expires: Mar 30 23:59:59 2027 GMT
  host: www.mirrorfly.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Mar 30 23:59:59 2027 GMT
  host: api-preprod-sandbox.mirrorfly.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mirrorfly Messages Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MirrorFly Messages API, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: MirrorFly Messages API
provider_slug: mirrorfly-messages-api
slug: mirrorfly-messages-api-domain-security
source_filename: mirrorfly-messages-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mirrorfly.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 30 23:59:59 2027 GMT\n  hsts: false\n- host: api-preprod-sandbox.mirrorfly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 30 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: mirrorfly.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mirrorfly-messages-api/refs/heads/main/security/mirrorfly-messages-api-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- CPaaS
- Communications
- Chat / Messaging API
- Voice API
- Video API
- SIP/VoIP
- Real-time Communication
- SDK
- Self-hosted / On-premise
- AI Agents / Chatbots
- Contact Center
---
