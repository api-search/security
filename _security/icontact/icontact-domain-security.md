---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: icontact.com
  spf: true
hosts:
- cert_expires: Sep 18 17:14:40 2026 GMT
  host: www.icontact.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 18 19:27:37 2026 GMT
  host: app.icontact.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Icontact Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for iContact, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: iContact
provider_slug: icontact
slug: icontact-domain-security
source_filename: icontact-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.icontact.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 17:14:40 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: app.icontact.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 19:27:37 2026 GMT\n  hsts: null\ndomains:\n- domain: icontact.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/icontact/refs/heads/main/security/icontact-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Email Marketing
- Marketing Automation
- Campaigns
- Contacts
- Lists
- SMB
---
