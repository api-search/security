---
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "sectigo.com"
  - 0 issue "amazontrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: monks.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mightyhive.com
  note: Legacy brand domain still under company control — SPF and a quarantine DMARC policy with an active rua address (dmarc-reports-mh@mightyhive.com) are still published, so the domain is maintained rather than abandoned. No DNSSEC and no CAA records.
  spf: true
hosts:
- cert_expires: Nov 24 23:59:59 2026 GMT
  host: www.monks.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 29 23:59:59 2026 GMT
  host: mightyhive.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  note: legacy MightyHive brand domain, added by hand from the same dig/openssl/HEAD probe
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mightyhive Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MightyHive, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: MightyHive
provider_slug: mightyhive
slug: mightyhive-domain-security
source_filename: mightyhive-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.monks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: mightyhive.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  note: legacy MightyHive brand domain, added by hand from the same dig/openssl/HEAD probe\ndomains:\n- domain: monks.com\n  dnssec: true\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: mightyhive.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n  note: >-\n    Legacy brand domain still under company control — SPF and a quarantine DMARC policy with\n    an active\
  \ rua address (dmarc-reports-mh@mightyhive.com) are still published, so the\n    domain is maintained rather than abandoned. No DNSSEC and no CAA records.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mightyhive/refs/heads/main/security/mightyhive-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Advertising
- Marketing
- Media
- Programmatic Advertising
- Consulting
- Data
- Advertising Technology
---
