---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  - 0 issue "amazontrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: verily.com
  spf: true
hosts:
- cert_expires: Nov 27 02:36:17 2026 GMT
  host: verily.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  1 00:34:47 2026 GMT
  host: support.workbench.verily.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 27 04:01:11 2026 GMT
  host: workbench.verily.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Verily Life Sciences Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Verily Life Sciences, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Verily Life Sciences
provider_slug: verily-life-sciences
slug: verily-life-sciences-domain-security
source_filename: verily-life-sciences-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: verily.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 02:36:17 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: support.workbench.verily.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 00:34:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: workbench.verily.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 04:01:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: verily.com\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/verily-life-sciences/refs/heads/main/security/verily-life-sciences-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Health
- Life Sciences
- Precision Health
- Clinical Research
- Biomedical Data
- FHIR
- Research Data Platform
- Trusted Research Environment
- Genomics
- Cloud Infrastructure
- Terraform
---
