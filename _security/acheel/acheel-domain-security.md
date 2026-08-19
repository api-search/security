---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: acheel.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: charlee.fr
  spf: true
hosts:
- cert_expires: Jan 18 23:59:59 2027 GMT
  host: www.acheel.com
  hsts: false
  https: true
  note: redirects to v2.acheel.com
  tls_version: TLSv1.3
- cert_expires: Sep 26 23:28:30 2026 GMT
  host: v2.acheel.com
  hsts: false
  https: true
  note: the live public website
  tls_version: TLSv1.3
- cert_expires: Dec 23 23:59:59 2026 GMT
  host: faq.acheel.com
  hsts: false
  https: true
  note: Intercom-hosted help centre on an Acheel hostname
  tls_version: TLSv1.3
- cert_expires: Oct 20 03:34:24 2026 GMT
  host: emprunteur.acheel.com
  hsts: false
  https: true
  note: borrower-insurance funnel
  tls_version: TLSv1.3
- cert_expires: Oct 18 23:21:51 2026 GMT
  host: www.charlee.fr
  hsts: false
  https: true
  note: Charlee broker brand marketing site
  tls_version: TLSv1.3
- cert_expires: Oct 25 23:27:12 2026 GMT
  host: back.charlee.fr
  hsts: false
  https: true
  note: Charlee broker portal ("Acheel Omega") — login-gated, no HSTS
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Acheel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Acheel, probed live across 6 host(s) and 2 registrable domain(s). 6 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Acheel
provider_slug: acheel
slug: acheel-domain-security
source_filename: acheel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of every Acheel and Charlee host reachable from public pages\nchecked: '2026-08-17'\nsummary: >-\n  Every host is HTTPS on TLS 1.3 with a valid certificate, but HSTS is enabled on none of them —\n  not on the public site, not on the borrower funnel, and not on the Charlee broker portal that\n  handles partner authentication. Both registrable domains publish SPF and DMARC, but neither\n  publishes DNSSEC or CAA, and charlee.fr's DMARC policy is p=none (monitor only) against\n  acheel.com's p=quarantine. RFC 9116 security.txt is absent everywhere (see well-known/).\nhosts:\n- host: www.acheel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 18 23:59:59 2027 GMT\n  hsts: false\n  note: redirects to v2.acheel.com\n- host: v2.acheel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 23:28:30 2026 GMT\n  hsts: false\n  note: the live public website\n- host: faq.acheel.com\n  https:\
  \ true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 23:59:59 2026 GMT\n  hsts: false\n  note: Intercom-hosted help centre on an Acheel hostname\n- host: emprunteur.acheel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 03:34:24 2026 GMT\n  hsts: false\n  note: borrower-insurance funnel\n- host: www.charlee.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 23:21:51 2026 GMT\n  hsts: false\n  note: Charlee broker brand marketing site\n- host: back.charlee.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 23:27:12 2026 GMT\n  hsts: false\n  note: 'Charlee broker portal (\"Acheel Omega\") — login-gated, no HSTS'\ndomains:\n- domain: acheel.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: charlee.fr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acheel/refs/heads/main/security/acheel-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Fintech Insurtech
- Insurance
- Insurtech
- Digital Insurance
- Home Insurance
- Auto Insurance
- Health Insurance
- Pet Insurance
- White Label
- B2B2C
- Embedded Insurance
- France
---
