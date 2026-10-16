---
description: ''
domains:
- caa:
  - 0 issue "harica.gr"
  - 0 issue "digicert.com"
  - 0 issuewild ";"
  - 0 issue "letsencrypt.org; accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/3660940211"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: riksdagen.se
  spf: true
hosts:
- cert_expires: Nov 28 11:46:35 2026 GMT
  host: riksdagen.se
  hsts: true
  hsts_max_age: 16070400
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Riksdagen Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Riksdagen, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Riksdagen
provider_slug: riksdagen
slug: riksdagen-domain-security
source_filename: riksdagen-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: riksdagen.se\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 11:46:35 2026 GMT\n  hsts: true\n  hsts_max_age: 16070400\ndomains:\n- domain: riksdagen.se\n  dnssec: true\n  caa:\n  - 0 issue \"harica.gr\"\n  - 0 issue \"digicert.com\"\n  - 0 issuewild \";\"\n  - 0 issue \"letsencrypt.org; accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/3660940211\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/riksdagen/refs/heads/main/security/riksdagen-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Government
- Sweden
- Legislature
- Politics
---
