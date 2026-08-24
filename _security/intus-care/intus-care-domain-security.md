---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: intuscare.com
  spf: true
  spf_record: v=spf1 include:spf.efwd.registrar-servers.com include:spf.easywp.com ~all
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dmarc_rua: present (address withheld)
  dmarc_subdomain_policy: quarantine
  dnssec: false
  domain: intus.care
  spf: true
  spf_record: v=spf1 include:spf.protection.outlook.com include:mail.zendesk.com include:49558872.spf07.hubspotemail.net -all
hosts:
- cert_expires: Oct  8 02:07:07 2026 GMT
  host: intuscare.com
  hsts: false
  https: true
  note: Every path on this host answers HTTP 202 with a SiteGround "sgcaptcha" JavaScript proof-of-work interstitial rather than the page, including /robots.txt and /llms.txt.
  role: marketing site (WordPress on SiteGround)
  tls_version: TLSv1.3
- cert_expires: Oct 24 12:22:53 2026 GMT
  host: intus.care
  hsts: true
  hsts_header: max-age=15552000; includeSubDomains
  hsts_preload: false
  https: true
  role: population health / IRIS analytics application (authenticated)
  tls_version: TLSv1.3
- cert_expires: Sep 18 23:59:59 2026 GMT
  host: carehub.intus.care
  hsts: true
  hsts_header: max-age=31536000; includeSubDomains; preload
  hsts_preload: true
  https: true
  role: CareHub EMR application (authenticated, Next.js)
  tls_version: TLSv1.3
- cert_expires: Sep 18 23:59:59 2026 GMT
  host: iris.intus.care
  hsts: true
  hsts_header: max-age=31536000; includeSubDomains; preload
  hsts_preload: true
  https: true
  role: IRIS risk adjustment application (authenticated)
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Intus Care Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Intus Care, probed live across 4 host(s) and 2 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Intus Care
provider_slug: intus-care
slug: intus-care-domain-security
source_filename: intus-care-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml hosts plus the two authenticated product\n  hosts discovered from the intuscare.com navigation (carehub.intus.care, intus.care)\nhosts:\n- host: intuscare.com\n  role: marketing site (WordPress on SiteGround)\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: 'Oct  8 02:07:07 2026 GMT'\n  hsts: false\n  note: >-\n    Every path on this host answers HTTP 202 with a SiteGround \"sgcaptcha\" JavaScript\n    proof-of-work interstitial rather than the page, including /robots.txt and /llms.txt.\n- host: intus.care\n  role: population health / IRIS analytics application (authenticated)\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: 'Oct 24 12:22:53 2026 GMT'\n  hsts: true\n  hsts_header: 'max-age=15552000; includeSubDomains'\n  hsts_preload: false\n- host: carehub.intus.care\n  role: CareHub EMR application (authenticated, Next.js)\n  https: true\n  tls_version: TLSv1.3\n  cert_expires:\
  \ 'Sep 18 23:59:59 2026 GMT'\n  hsts: true\n  hsts_header: 'max-age=31536000; includeSubDomains; preload'\n  hsts_preload: true\n- host: iris.intus.care\n  role: IRIS risk adjustment application (authenticated)\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: 'Sep 18 23:59:59 2026 GMT'\n  hsts: true\n  hsts_header: 'max-age=31536000; includeSubDomains; preload'\n  hsts_preload: true\ndomains:\n- domain: intuscare.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: 'v=spf1 include:spf.efwd.registrar-servers.com include:spf.easywp.com ~all'\n  dmarc: true\n  dmarc_policy: none\n- domain: intus.care\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: 'v=spf1 include:spf.protection.outlook.com include:mail.zendesk.com include:49558872.spf07.hubspotemail.net -all'\n  dmarc: true\n  dmarc_policy: quarantine\n  dmarc_subdomain_policy: quarantine\n  dmarc_rua: present (address withheld)\nfindings:\n- Both product hosts (carehub, iris) send HSTS with includeSubDomains and preload;\
  \ the\n  marketing host sends no HSTS at all.\n- Neither domain publishes a CAA record and neither is DNSSEC-signed.\n- intus.care enforces SPF with a hard fail (-all) and a DMARC quarantine policy;\n  intuscare.com uses a soft-fail SPF (~all) and p=none, so the marketing domain is the\n  weaker of the two for spoofing.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/intus-care/refs/heads/main/security/intus-care-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Health Care
- Electronic Health Records
- Population Health
- Risk Adjustment
- Senior Care
- Value-Based Care
- Analytics
- Compliance
- Utilization Management
- PACE
---
