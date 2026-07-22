---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "www.digicert.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: plexus.com
  spf: true
hosts:
- cert_expires: Sep 11 23:59:59 2026 GMT
  host: www.plexus.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Plexus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Plexus, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Plexus
provider_slug: plexus
slug: plexus-domain-security
source_filename: plexus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.plexus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: plexus.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"www.digicert.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/plexus/refs/heads/main/security/plexus-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Aerospace
- Defense
- Healthcare
- Industrial
- Manufacturing
- Product Development
- Semiconductor
- Supply Chain
- Fortune 1000
---
