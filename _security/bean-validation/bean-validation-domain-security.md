---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: beanvalidation.org
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hibernate.org
  spf: true
hosts:
- cert_expires: Sep 20 17:02:52 2026 GMT
  host: beanvalidation.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 19:49:12 2026 GMT
  host: hibernate.org
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 01:24:39 2026 GMT
  host: jakarta.ee
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bean Validation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bean Validation, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Bean Validation
provider_slug: bean-validation
slug: bean-validation-domain-security
source_filename: bean-validation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: beanvalidation.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 17:02:52 2026 GMT\n  hsts: false\n- host: hibernate.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 19:49:12 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: jakarta.ee\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 01:24:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: beanvalidation.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n- domain: hibernate.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bean-validation/refs/heads/main/security/bean-validation-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Bean Validation
- Data Quality
- Java
- Validation
- Jakarta EE
- Constraints
---
