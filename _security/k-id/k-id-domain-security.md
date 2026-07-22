---
description: ''
domains:
- caa:
  - 0 issue "awstrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: k-id.com
  spf: true
hosts:
- cert_expires: Mar 12 23:59:59 2027 GMT
  host: docs.k-id.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 17 03:04:37 2026 GMT
  host: game-api.k-id.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: K Id Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for k-ID, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: k-ID
provider_slug: k-id
slug: k-id-domain-security
source_filename: k-id-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.k-id.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 12 23:59:59 2027 GMT\n  hsts: false\n- host: game-api.k-id.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 03:04:37 2026 GMT\n  hsts: null\ndomains:\n- domain: k-id.com\n  dnssec: false\n  caa:\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/k-id/refs/heads/main/security/k-id-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Age Verification
- Age Assurance
- Compliance
- Parental Consent
- Child Safety
- Identity
- Privacy
- Regulatory Technology
- Gaming
---
