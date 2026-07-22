---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "letsencrypt.org"
  - 0 issuewild ";"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: freenome.com
  spf: true
hosts:
- cert_expires: Oct 10 09:43:48 2026 GMT
  host: www.freenome.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Freenome Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Freenome, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Freenome
provider_slug: freenome
slug: freenome-domain-security
source_filename: freenome-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.freenome.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 09:43:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: freenome.com\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \";\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/freenome/refs/heads/main/security/freenome-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Healthcare
- Cancer Detection
- Diagnostics
- Life Sciences
- Artificial Intelligence
- Machine Learning
- Multiomics
- Clinical Screening
---
