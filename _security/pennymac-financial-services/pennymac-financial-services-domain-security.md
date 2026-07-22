---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: pennymacfinancial.com
  spf: true
- caa:
  - 0 iodef "mailto:Cyrus.Tibbs@pennymac.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "awstrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: pennymac.com
  spf: true
hosts:
- cert_expires: Aug 23 14:28:04 2026 GMT
  host: www.pennymacfinancial.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 13:14:17 2026 GMT
  host: pfsi.pennymac.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pennymac Financial Services Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PennyMac Financial Services, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: PennyMac Financial Services
provider_slug: pennymac-financial-services
slug: pennymac-financial-services-domain-security
source_filename: pennymac-financial-services-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pennymacfinancial.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 14:28:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: pfsi.pennymac.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 13:14:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: pennymacfinancial.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: pennymac.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:Cyrus.Tibbs@pennymac.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"awstrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pennymac-financial-services/refs/heads/main/security/pennymac-financial-services-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial Services
- Mortgage
- Lending
- Real Estate
---
