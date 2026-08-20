---
description: ''
domains:
- caa: []
  dmarc: false
  dmarc_policy: null
  dnssec: false
  domain: epicsciences.com
  mx: []
  note: No MX record, no SPF TXT record and no _dmarc TXT record. A domain with no published email authentication policy that no longer resolves to its owner's infrastructure is spoofable; this is recorded as observed fact, not as a finding attributed to Epic Sciences' current operations.
  spf: false
hosts:
- cert_expires: '2026-10-18'
  cert_issuer: Let's Encrypt
  cert_not_before: '2026-07-20'
  host: www.epicsciences.com
  hsts: false
  hsts_max_age: null
  http_status: 301
  https: true
  note: Every path probed returns 301 to an unrelated off-domain host, including /robots.txt, /sitemap.xml and every /.well-known/ path.
  redirects_to: https://www.awaji-musicisland.com/
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Epic Sciences Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Epic Sciences, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Epic Sciences
provider_slug: epic-sciences
slug: epic-sciences-domain-security
source_filename: epic-sciences-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of epicsciences.com (the company's registered domain)\nnote: >-\n  Probed against epicsciences.com, the domain every third-party record (LinkedIn,\n  Wikipedia, Tracxn, ZoomInfo) still lists as the Epic Sciences website. The\n  earlier automated pass probed forgeglobal.com, which is the secondary-market\n  listing broker carried in apis.yml common[] as the harvest source, not a host\n  Epic Sciences operates; those results were removed rather than attributed here.\n  The domain is registered through 2027-08-30 (GoDaddy, Cloudflare nameservers)\n  and holds a valid Let's Encrypt certificate re-issued 2026-07-20, but it serves\n  a blanket HTTP 301 to an unrelated third-party site and publishes no MX, SPF,\n  DMARC, CAA or DNSSEC records — i.e. the company no longer operates web or email\n  on its own domain.\nhosts:\n- host: www.epicsciences.com\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: \"\
  Let's Encrypt\"\n  cert_not_before: '2026-07-20'\n  cert_expires: '2026-10-18'\n  hsts: false\n  hsts_max_age: null\n  http_status: 301\n  redirects_to: https://www.awaji-musicisland.com/\n  note: >-\n    Every path probed returns 301 to an unrelated off-domain host, including\n    /robots.txt, /sitemap.xml and every /.well-known/ path.\ndomains:\n- domain: epicsciences.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n  dmarc_policy: null\n  mx: []\n  note: >-\n    No MX record, no SPF TXT record and no _dmarc TXT record. A domain with no\n    published email authentication policy that no longer resolves to its owner's\n    infrastructure is spoofable; this is recorded as observed fact, not as a\n    finding attributed to Epic Sciences' current operations.\nx-evidence:\n- url: https://www.epicsciences.com/\n  status: 301\n  observed: '2026-08-12'\n- url: https://www.epicsciences.com/robots.txt\n  status: 301\n  observed: '2026-08-12'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/epic-sciences/refs/heads/main/security/epic-sciences-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Healthcare
- Diagnostics
- Oncology
- Life Sciences
- Biotechnology
- Laboratory
- Precision Medicine
---
