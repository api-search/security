---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: jhilburn.com
  spf: true
hosts:
- cert_expires: Oct 31 09:06:15 2026 GMT
  host: jhilburn.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 13:24:54 2026 GMT
  host: api.jhilburn.com
  hsts: null
  https: true
  note: Live dedicated origin (Microsoft-IIS/8.5, X-Powered-By ASP.NET) that answers 403 at / and 404 on every documentation path probed. No HSTS header. Not fronted by the CDN that fronts jhilburn.com.
  tls_version: TLSv1.2
- cert_expires: Oct  7 14:32:28 2026 GMT
  host: stylist.jhilburn.com
  hsts: max-age=15552000
  https: true
  note: Stylist recruiting/training site. HSTS present without includeSubDomains or preload.
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: J Hilburn Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for J Hilburn, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: J Hilburn
provider_slug: j-hilburn
slug: j-hilburn-domain-security
source_filename: j-hilburn-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml hosts, plus hand-probed api.jhilburn.com and stylist.jhilburn.com\n  (2026-08-23)\nhosts:\n- host: jhilburn.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 09:06:15 2026 GMT\n  hsts: null\n- host: api.jhilburn.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 29 13:24:54 2026 GMT\n  hsts: null\n  note: Live dedicated origin (Microsoft-IIS/8.5, X-Powered-By ASP.NET) that answers 403 at / and 404\n    on every documentation path probed. No HSTS header. Not fronted by the CDN that fronts jhilburn.com.\n- host: stylist.jhilburn.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  7 14:32:28 2026 GMT\n  hsts: max-age=15552000\n  note: Stylist recruiting/training site. HSTS present without includeSubDomains or preload.\ndomains:\n- domain: jhilburn.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/j-hilburn/refs/heads/main/security/j-hilburn-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Retail
- Apparel
- Fashion
- Ecommerce
- Direct to Consumer
- Menswear
- Custom Clothing
---
