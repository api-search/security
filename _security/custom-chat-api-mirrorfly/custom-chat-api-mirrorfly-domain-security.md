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
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Custom Chat Api Mirrorfly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Custom Chat API | MirrorFly, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Custom Chat API | MirrorFly
provider_slug: custom-chat-api-mirrorfly
slug: custom-chat-api-mirrorfly-domain-security
source_filename: custom-chat-api-mirrorfly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mirrorfly.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 30 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: mirrorfly.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/custom-chat-api-mirrorfly/refs/heads/main/security/custom-chat-api-mirrorfly-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Chat API
- Messaging
- CPaaS
- VoIP
- Voice
- Video Calling
- Contact Center
- Conversational AI
- Chatbots
- Live Streaming
---
