---
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 iodef "mailto:devops_team+caa@fetcherr.io"
  - 0 issuewild "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: fetcherr.io
  spf: true
hosts:
- cert_expires: Sep 15 18:36:31 2026 GMT
  host: www.fetcherr.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fetcherr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fetcherr, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Fetcherr
provider_slug: fetcherr
slug: fetcherr-domain-security
source_filename: fetcherr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fetcherr.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 18:36:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: fetcherr.io\n  dnssec: true\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 iodef \"mailto:devops_team+caa@fetcherr.io\"\n  - 0 issuewild \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fetcherr/refs/heads/main/security/fetcherr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Aviation
- Airlines
- Dynamic Pricing
- Revenue Management
- Generative AI
- Travel
- Pricing
---
