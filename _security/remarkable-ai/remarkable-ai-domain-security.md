---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dmarc_record: v=DMARC1; p=none; rua=mailto:aneto@beremarkable.ai
  dnssec: false
  domain: beremarkable.ai
  role: current brand
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: reject
  dmarc_record: v=DMARC1; p=reject; sp=none; pct=100; ri=86400; rua=mailto:info@chatdesk.com
  dnssec: false
  domain: chatdesk.com
  role: legacy brand
  spf: true
  spf_record: v=spf1 include:_spf.google.com ~all include:2225701.spf06.hubspotemail.net
hosts:
- cert_expires: Sep 19 18:31:33 2026 GMT
  host: www.beremarkable.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  role: marketing website
  tls_version: TLSv1.3
- host: app.beremarkable.ai
  hsts: false
  https: true
  role: customer application (SPA)
  tls_version: TLSv1.3
- host: help.beremarkable.ai
  hsts: false
  https: true
  role: help center (Intercom-hosted)
  tls_version: TLSv1.3
- host: www.chatdesk.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  role: legacy brand marketing website
  tls_version: TLSv1.3
- host: api.chatdesk.com
  hsts: false
  https: true
  role: internal backend (AWS API Gateway)
  tls_version: TLSv1.3
- host: trends.chatdesk.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  role: Trends application (Spring Boot)
  tls_note: Negotiates TLS 1.2 only; the other six hosts all reach TLS 1.3. Not a defect, but it is the weakest transport posture in the estate.
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Remarkable Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Remarkable AI, probed live across 6 host(s) and 2 registrable domain(s). 6 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Remarkable AI
provider_slug: remarkable-ai
slug: remarkable-ai-domain-security
source_filename: remarkable-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: >-\n  Live DNS/TLS/HTTP probes. apis.yml carries no apis[] and no baseURL, so\n  probe-domain-security.py could only reach www.beremarkable.ai; the remaining hosts and\n  the second domain were probed directly during contract discovery and folded in here.\nchecked: '2026-08-13'\n\nhosts:\n- host: www.beremarkable.ai\n  role: marketing website\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 18:31:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n\n- host: app.beremarkable.ai\n  role: customer application (SPA)\n  https: true\n  tls_version: TLSv1.3\n  hsts: false\n\n- host: help.beremarkable.ai\n  role: help center (Intercom-hosted)\n  https: true\n  tls_version: TLSv1.3\n  hsts: false\n\n- host: www.chatdesk.com\n  role: legacy brand marketing website\n  https: true\n  tls_version: TLSv1.3\n  hsts: true\n  hsts_max_age: 31536000\n\n- host: api.chatdesk.com\n  role: internal backend (AWS API Gateway)\n  https:\
  \ true\n  tls_version: TLSv1.3\n  hsts: false\n\n- host: trends.chatdesk.com\n  role: Trends application (Spring Boot)\n  https: true\n  tls_version: TLSv1.2\n  tls_note: >-\n    Negotiates TLS 1.2 only; the other six hosts all reach TLS 1.3. Not a defect, but it\n    is the weakest transport posture in the estate.\n  hsts: true\n  hsts_max_age: 31536000\n\ndomains:\n- domain: beremarkable.ai\n  role: current brand\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n  dmarc_record: 'v=DMARC1; p=none; rua=mailto:aneto@beremarkable.ai'\n\n- domain: chatdesk.com\n  role: legacy brand\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: 'v=spf1 include:_spf.google.com ~all include:2225701.spf06.hubspotemail.net'\n  dmarc: true\n  dmarc_policy: reject\n  dmarc_record: 'v=DMARC1; p=reject; sp=none; pct=100; ri=86400; rua=mailto:info@chatdesk.com'\n\nfindings:\n- id: email-auth-regressed-on-rebrand\n  severity: notable\n  summary: >-\n    The current brand's domain\
  \ is weaker at email authentication than the brand it\n    replaced. beremarkable.ai publishes NO SPF record at all and a DMARC policy of\n    p=none (monitor only). The legacy chatdesk.com publishes both an SPF record and\n    DMARC p=reject. This is worth flagging because 1:1 email delivery — including\n    \"primary inbox delivery\" — is the product this company sells; the domain carrying\n    the new brand is the one with no SPF and no enforcing DMARC.\n  evidence:\n  - 'dig TXT beremarkable.ai -> no v=spf1 record'\n  - 'dig TXT _dmarc.beremarkable.ai -> v=DMARC1; p=none'\n  - 'dig TXT chatdesk.com -> v=spf1 include:_spf.google.com ~all'\n  - 'dig TXT _dmarc.chatdesk.com -> v=DMARC1; p=reject'\n- id: no-caa-no-dnssec\n  severity: minor\n  summary: >-\n    Neither domain publishes CAA records or is DNSSEC-signed, so certificate issuance is\n    unconstrained and DNS answers are unauthenticated. Common across the catalog.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/remarkable-ai/refs/heads/main/security/remarkable-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Applicative Saas
- Customer Engagement
- Personalization
- E-Commerce
- Artificial Intelligence
- Customer-Support
- Marketing
---
