---
description: ''
domains:
- caa:
  - 0 issuewild "amazon.com"
  - 0 issue "globalsign.com"
  - 0 issuewild "globalsign.com"
  - 0 issuewild "identrust.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: true
  domain: nih.gov
  spf: false
hosts:
- cert_expires: Sep 15 15:25:27 2026 GMT
  host: www.niams.nih.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: National Institute Of Arthritis And Musculoskeletal And Skin Diseases Niams  Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for National Institute of Arthritis and Musculoskeletal and Skin Diseases (NIAMS), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: National Institute of Arthritis and Musculoskeletal and Skin Diseases (NIAMS)
provider_slug: national-institute-of-arthritis-and-musculoskeletal-and-skin-diseases-niams-
slug: national-institute-of-arthritis-and-musculoskeletal-and-skin-diseases-niams--domain-security
source_filename: national-institute-of-arthritis-and-musculoskeletal-and-skin-diseases-niams--domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.niams.nih.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 15:25:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nih.gov\n  dnssec: true\n  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issuewild \"globalsign.com\"\n  - 0 issuewild \"identrust.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"letsencrypt.org\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/national-institute-of-arthritis-and-musculoskeletal-and-skin-diseases-niams-/refs/heads/main/security/national-institute-of-arthritis-and-musculoskeletal-and-skin-diseases-niams--domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Federal Government
- Health
- NIH
- Research
---
