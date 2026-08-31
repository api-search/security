---
description: ''
domains:
- caa:
  - 0 issue "globalsign.com"
  - 0 issuewild "globalsign.com"
  - 0 issue "digicert.com"
  - 0 issuewild "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: turborater.com
  spf: true
- caa:
  - 0 issuewild "digicert.com"
  - 0 issuewild "globalsign.com"
  - 0 issuewild "pki.goog"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: zywave.com
  spf: true
hosts:
- cert_expires: Sep 24 12:46:31 2026 GMT
  host: www.turborater.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug 25 01:53:45 2026 GMT
  host: www.zywave.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Turborater Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TurboRater, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: TurboRater
provider_slug: turborater
slug: turborater-domain-security
source_filename: turborater-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.turborater.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 24 12:46:31 2026 GMT\n  hsts: false\n- host: www.zywave.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 01:53:45 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: turborater.com\n  dnssec: false\n  caa:\n  - 0 issue \"globalsign.com\"\n  - 0 issuewild \"globalsign.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: zywave.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"globalsign.com\"\n  - 0 issuewild \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/turborater/refs/heads/main/security/turborater-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Insurance
- InsurTech
- Comparative Rating
- Auto Insurance
- Home Insurance
- Quotes
- Real-Time Rating
- Personal Lines
- ITC
- Zywave
---
