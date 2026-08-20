---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: optinmonster.com
  spf: true
- caa:
  - 0 iodef "mailto:caa@wordpress.org"
  - 0 issue "letsencrypt.org;validationmethods=dns-01;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/53691143"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wordpress.org
  spf: true
hosts:
- cert_expires: Sep 14 15:35:11 2026 GMT
  host: optinmonster.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 05:52:12 2026 GMT
  host: api.optinmonster.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 23 19:43:55 2026 GMT
  host: wordpress.org
  hsts: true
  hsts_max_age: 3600
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Optinmonster Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OptinMonster, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: OptinMonster
provider_slug: optinmonster
slug: optinmonster-domain-security
source_filename: optinmonster-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: optinmonster.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 15:35:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.optinmonster.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 05:52:12 2026 GMT\n  hsts: false\n- host: wordpress.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 19:43:55 2026 GMT\n  hsts: true\n  hsts_max_age: 3600\ndomains:\n- domain: optinmonster.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: wordpress.org\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:caa@wordpress.org\"\n  - 0 issue \"letsencrypt.org;validationmethods=dns-01;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/53691143\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/optinmonster/refs/heads/main/security/optinmonster-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Lead Generation
- Marketing
- Conversion Optimization
- Email Marketing
- Popups
- WordPress
- Webhook
- Software-as-a-Service
- Marketing Automation
---
