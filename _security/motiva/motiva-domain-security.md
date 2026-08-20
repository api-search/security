---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: motiva.ai
  spf: true
hosts:
- cert_expires: Nov 11 10:47:12 2026 GMT
  host: www.motiva.ai
  hsts: false
  https: true
  note: Answers HTTP 202 with a SiteGround bot-challenge interstitial on every path, including /robots.txt.
  role: marketing site
  tls_version: TLSv1.3
- cert_expires: Nov  2 05:25:38 2026 GMT
  host: app.motiva.ai
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_preload: true
  https: true
  note: The only Motiva host that sets HSTS. Two Strict-Transport-Security headers are returned (max-age=31536000 includeSubDomains preload, and max-age=15724800 includeSubdomains) — a duplicated header, likely one from the app and one from the edge.
  role: customer application
  tls_version: TLSv1.3
- cert_expires: Dec 13 23:59:59 2026 GMT
  host: api.motiva.ai
  hsts: false
  https: true
  note: Returns HTTP 403 {"message":"Forbidden"} on every anonymous path.
  role: application backend (AWS-fronted)
  tls_version: TLSv1.3
- cert_expires: Oct 21 23:59:59 2026 GMT
  host: help.plugin.motiva.ai
  hsts: false
  https: true
  note: 302 on the root; serves llms.txt and a security.txt (Intercom's) at 200.
  role: Help Center (Intercom-hosted)
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Motiva Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Motiva, probed live across 4 host(s) and 1 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Motiva
provider_slug: motiva
slug: motiva-domain-security
source_filename: motiva-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: >-\n  live DNS/TLS/HTTP probes of apis.yml hosts (0-working/probe-domain-security.py),\n  extended by hand with the three additional Motiva-controlled hosts found during\n  contract discovery: api.motiva.ai, app.motiva.ai and help.plugin.motiva.ai.\nhosts:\n- host: www.motiva.ai\n  role: marketing site\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 10:47:12 2026 GMT\n  hsts: false\n  note: >-\n    Answers HTTP 202 with a SiteGround bot-challenge interstitial on every path,\n    including /robots.txt.\n- host: app.motiva.ai\n  role: customer application\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 05:25:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  hsts_preload: true\n  note: >-\n    The only Motiva host that sets HSTS. Two Strict-Transport-Security headers are\n    returned (max-age=31536000 includeSubDomains preload, and max-age=15724800\n    includeSubdomains)\
  \ — a duplicated header, likely one from the app and one from the edge.\n- host: api.motiva.ai\n  role: application backend (AWS-fronted)\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 23:59:59 2026 GMT\n  hsts: false\n  note: Returns HTTP 403 {\"message\":\"Forbidden\"} on every anonymous path.\n- host: help.plugin.motiva.ai\n  role: Help Center (Intercom-hosted)\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 23:59:59 2026 GMT\n  hsts: false\n  note: 302 on the root; serves llms.txt and a security.txt (Intercom's) at 200.\ndomains:\n- domain: motiva.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/motiva/refs/heads/main/security/motiva-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Marketing
- Email Marketing
- Marketing Automation
- Artificial Intelligence
- Machine-Learning
- Generative AI
- Oracle Eloqua
- Personalization
---
