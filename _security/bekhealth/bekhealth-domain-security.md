---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: bekhealth.com
  spf: true
hosts:
- cert_expires: Oct 10 22:09:51 2026 GMT
  host: www.bekhealth.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 18:41:40 2026 GMT
  host: auth.bekhealth.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  note: Auth0 custom-domain OIDC issuer, fronted by Cloudflare.
  tls_version: TLSv1.3
- cert_expires: Feb  8 23:59:59 2027 GMT
  host: docs.bekhealth.com
  hsts: false
  https: true
  note: CloudFront-fronted documentation portal; every path 302s to the Auth0 issuer.
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bekhealth Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BEKHealth, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: BEKHealth
provider_slug: bekhealth
slug: bekhealth-domain-security
source_filename: bekhealth-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bekhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 22:09:51 2026 GMT\n  hsts: false\n- host: auth.bekhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 18:41:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  note: Auth0 custom-domain OIDC issuer, fronted by Cloudflare.\n- host: docs.bekhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  8 23:59:59 2027 GMT\n  hsts: false\n  note: CloudFront-fronted documentation portal; every path 302s to the Auth0 issuer.\ndomains:\n- domain: bekhealth.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bekhealth/refs/heads/main/security/bekhealth-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Healthcare
- Clinical Trials
- Clinical Research
- Electronic Health Records
- Real-World Data
- Artificial Intelligence
- Patient Recruitment
- Life Sciences
- Health Data
---
