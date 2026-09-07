---
description: ''
domains:
- caa:
  - 0 issue "vikingcloud.com"
  - 0 issue "ssl.com"
  - 0 issue "securetrust.com"
  - 0 issue "pki.goog"
  - 0 issuewild "ssl.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: 247.ai
  spf: true
- caa:
  - 0 bissue "trustwave.com"
  - 0 bissuewild "trustwave.com"
  - 0 bissue "ssl.com"
  - 0 bissuewild "ssl.com"
  - 0 bissue "godaddy.com"
  dmarc: true
  dmarc_policy: reject
  dmarc_subdomain_policy: none
  dnssec: false
  domain: 247-inc.net
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dmarc_subdomain_policy: reject
  dnssec: false
  domain: 247-inc.com
  spf: true
hosts:
- cert_expires: Oct 29 23:59:59 2026 GMT
  host: www.247.ai
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  8 04:06:07 2026 GMT
  host: login.247.ai
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 315360000
  https: true
  note: Okta-hosted [24]7 Engagement Cloud SSO tenant; serves OIDC + OAuth 2.0 discovery.
  tls_version: TLSv1.2
- cert_expires: Feb  5 12:33:19 2027 GMT
  host: api.247-inc.net
  hsts: false
  http_status: 503
  https: true
  note: Wildcard certificate CN=*.api.247-inc.net (SSL.com, issued 2026-02-05). Apex returns 503 from the load balancer; production traffic is per-tenant on subdomains.
  tls_version: TLSv1.3
- cert_expires: Jan  9 10:45:01 2027 GMT
  host: ph-chat.247-inc.com
  hsts: false
  http_status: 200
  https: true
  note: Philippines chat/ChatbotAI console login host.
  tls_version: TLSv1.3
hosts_probed: 4
kind: domain-security
layout: security
method: probed
name: 247 Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for [24]7.ai, probed live across 4 host(s) and 3 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: '[24]7.ai'
provider_slug: 247-ai
slug: 247-ai-domain-security
source_filename: 247-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + related [24]7.ai production hosts\nnote: >-\n  Baseline written by 0-working/probe-domain-security.py (www.247.ai + 247.ai). The\n  login.247.ai, api.247-inc.net and ph-chat.247-inc.com rows, and the 247-inc.net /\n  247-inc.com domain rows, were probed by hand with the same method (openssl s_client for\n  TLS version + cert expiry, HEAD for HSTS, dig for DNSSEC/CAA/SPF/DMARC) because apis[] is\n  empty for this provider and the script only walks apis.yml API hosts. api.247-inc.net is\n  [24]7.ai's tenant-routed production API host; its apex answers 503 from the load balancer.\nhosts:\n- host: www.247.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: login.247.ai\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  8 04:06:07 2026 GMT\n  hsts: true\n  hsts_max_age: 315360000\n  hsts_include_subdomains:\
  \ true\n  note: Okta-hosted [24]7 Engagement Cloud SSO tenant; serves OIDC + OAuth 2.0 discovery.\n- host: api.247-inc.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  5 12:33:19 2027 GMT\n  hsts: false\n  http_status: 503\n  note: >-\n    Wildcard certificate CN=*.api.247-inc.net (SSL.com, issued 2026-02-05). Apex returns 503\n    from the load balancer; production traffic is per-tenant on subdomains.\n- host: ph-chat.247-inc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 10:45:01 2027 GMT\n  hsts: false\n  http_status: 200\n  note: Philippines chat/ChatbotAI console login host.\ndomains:\n- domain: 247.ai\n  dnssec: false\n  caa:\n  - 0 issue \"vikingcloud.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issue \"securetrust.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: 247-inc.net\n  dnssec: false\n  caa:\n  - 0 bissue \"trustwave.com\"\n  - 0 bissuewild\
  \ \"trustwave.com\"\n  - 0 bissue \"ssl.com\"\n  - 0 bissuewild \"ssl.com\"\n  - 0 bissue \"godaddy.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n  dmarc_subdomain_policy: none\n- domain: 247-inc.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n  dmarc_subdomain_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/247-ai/refs/heads/main/security/247-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Customer Experience
- Conversational AI
- Contact Center
- Customer Service
- Chatbots
- CCaaS
- Artificial Intelligence
- Interaction Analytics
- Business Process Outsourcing
---
