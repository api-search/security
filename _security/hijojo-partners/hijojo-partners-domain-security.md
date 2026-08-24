---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: hijojo-partners.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hijojo.com
  spf: true
hosts:
- cert_expires: Oct 16 23:59:59 2026 GMT
  host: www.hijojo-partners.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 29 14:59:00 2026 GMT
  host: www.hijojo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  include_subdomains: false
  tls_version: TLSv1.3
- cert_expires: Dec 29 14:59:00 2026 GMT
  host: members.hijojo.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  include_subdomains: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hijojo Partners Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HiJoJo Partners, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: HiJoJo Partners
provider_slug: hijojo-partners
slug: hijojo-partners-domain-security
source_filename: hijojo-partners-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hijojo-partners.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 23:59:59 2026 GMT\n  hsts: false\n- host: www.hijojo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 14:59:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  include_subdomains: false\n- host: members.hijojo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 14:59:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\n  include_subdomains: true\ndomains:\n- domain: hijojo-partners.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: hijojo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\nnote: 'Extended beyond the apis.yml Website host: the retail platform (www.hijojo.com)\n  and the authenticated member application (members.hijojo.com) were probed directly\n  on 2026-08-22. Both\
  \ serve HSTS; the corporate Webflow site does not. hijojo-partners.com\n  publishes SPF but no DMARC record; hijojo.com publishes DMARC p=quarantine. Neither\n  domain is DNSSEC-signed and neither publishes a CAA record.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hijojo-partners/refs/heads/main/security/hijojo-partners-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Financial Services
- Investment Management
- Private Markets
- Secondary Markets
- Pre-IPO
- Venture Capital
- Fintech
- Japan
- Asset Management
---
